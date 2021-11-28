<template>
	<div class="stickyheader-container" :class="{nav_colored: scrollPosition > 200}">
		<div class="nav-container">
		<div class="nav-left">
			<div class="logo-container">
			<div class="left-logo">
				<div class="background-logo"></div>
				<h1>NEX</h1>
			</div>
			<div class="right-logo">
				<h1>GEN</h1>
			</div>
			</div>
		</div>
		<div class="nav-right">
			<a href="#">HOME</a>
			<a id="scrollAbout">ABOUT</a>
			<a id="scrollServices">SERVICES</a>
			<a id="scrollPricing">PRICING</a>
			<a id="scrollBlog">BLOG</a>
			<a id="scrollTouch" class="btn">GET IN TOUCH</a>
		</div>
		</div>
	</div>
</template>

<script>
export default {
  name: "stickyHeader",
    data() {
        return{
            scrollPosition: null
        }
    },
    mounted() {
        window.addEventListener('scroll', this.updateScroll);
        let about = document.getElementById('scrollAbout')
        about.addEventListener('click', this.scrollAbout)
        let services = document.getElementById('scrollServices')
        services.addEventListener('click', this.scrollServices)
        let pricing = document.getElementById('scrollPricing')
        pricing.addEventListener('click', this.scrollPricing)
        let blog = document.getElementById('scrollBlog')
        blog.addEventListener('click', this.scrollBlog)
        let touch = document.getElementById('scrollTouch')
        touch.addEventListener('click', this.scrollTouch)
    },
    methods: {
        updateScroll() {
            this.scrollPosition = window.scrollY
        },
        scrollAbout(){
            window.scrollTo(0, document.getElementById('about').offsetTop-50);
        },
        scrollServices(){
            window.scrollTo(0, document.getElementById('services').offsetTop-50);
        },
        scrollPricing(){
            window.scrollTo(0, document.getElementById('pricing').offsetTop-50);
        },
        scrollBlog(){
            window.scrollTo(0, document.getElementById('blog').offsetTop-50);
        },
        scrollTouch(){
            window.scrollTo(0, document.getElementById('touch').offsetTop-50);
        }
    }   
};
</script>

<style lang="scss">
@import '../assets/scss/common.scss';

.stickyheader-container{
	display: flex;
	justify-content: center;
	position: sticky;
	top: -1px;
	z-index: 3;
	width: 100%;
	transition: all 0.3s;
	background-color: transparent;

	.nav-container{
		display: flex;
		justify-content: space-between;
		width: 75%;
		height: 50px;
		z-index: 1;
		align-items: center;
		margin: 1rem 0;

		.nav-left{

			.logo-container{
				display: flex;
				font-weight: 900;
				align-items: center;

				.left-logo{
					color: $site_green;
					position: relative;
					display: flex;
					padding-left: 1.5rem;
					font-weight: 900;
					
					.background-logo{
						position: absolute;
						height: 100%;
						width: 100%;
						background-color: $site_green;
						filter: opacity(0.3);
						left: 0;
						border-top-left-radius: 25px;
						border-bottom-left-radius: 25px;
					}

					h1{
						padding-right: 0.5rem;
					}
				}
			}
		}

		.nav-right{
			display: flex;
			align-items: center;
			height: 100%;

			a{
				text-decoration: none;
				color: #e3e7df;
				padding: 0 1rem;
				font-weight: 900;
				cursor: pointer;

				&:hover{
					color: $site_green;
				}
			}

			.btn{
				padding: 0.5rem 1rem;
				color: #e3e7df !important;
			}
		}
	}
}
</style>