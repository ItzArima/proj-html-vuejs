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
        <a id="home">HOME</a>
        <a href="#about">ABOUT</a>
        <a href="#services">SERVICES</a>
        <a href="#pricing">PRICING</a>
        <a href="#blog">BLOG</a>
        <a href="#touch" class="btn">GET IN TOUCH</a>
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
        let home = document.getElementById('home')
        home.addEventListener('click',this.goTop);
    },
    methods: {
        updateScroll() {
            this.scrollPosition = window.scrollY
        },
        goTop() {
          document.body.scrollTop = 0,
          document.documentElement.scrollTop = 0
        }
    }   
};
</script>

<style lang="scss">

</style>