<template>
    <div class="newsletter-container">
        <div class="newsletter-centered">
            <div class="newsletter-left">
                <p class="green">NEWSLETTER</p>
                <div class="newsletter-title">
                    <div class="title-left">
                        <div class="title-bg"></div>
                        <h1 class="hidden">Know</h1>
                        <h1 class="absolute">Know</h1>
                    </div>
                    <div class="title-right">
                        <h1>First</h1>
                    </div>
                </div>
                <div class="newsletter-text">
                    <p>Followed closely and receive content about our company
                        and the news of the current market.
                    </p>
                </div>
            </div>
            <div class="newsletter-right">
                <form action="#">
                    <input type="text" id="name" name="name" placeholder="Name">
                    <input type="text" id="mail" name="mail" placeholder="Email">
                    <button class="btn">Subscribe</button>
                </form> 
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name : 'newsletter'
}
</script>

<style lang="scss">
@import '../assets/scss/common.scss';

.newsletter-container{
    display: flex;
    justify-content: center;
    background-image: url('../assets/img/bg-1.jpg');
    padding: 5rem 0;
    background-position: center;
    background-size: cover;
    background-attachment: fixed;

    .newsletter-centered{
        width: 75%;
        display: flex;

        .newsletter-left{
            width: 50%;
            margin-right: 1rem;

            .green{
                color: $site_green;
                margin-bottom: 1rem;
            }

            .newsletter-title{
                display: flex;
                margin-bottom: 2rem;

                .title-left{
                    position: relative;

                    .absolute{
                        position: absolute;
                        top: 0;
                        padding-left: 0.5rem;
                    }

                    .hidden{
                        visibility: hidden;
                        padding: 0 0.5rem;
                    }

                    .title-bg{
                        background-color: $site_green;
                        filter: opacity(0.3);
                        height: 100%;
                        width: 100%;
                    }
                }
            }
        }

        .newsletter-right{
            width: 50%;
            margin-left: 1rem;
            
            input{
                width: 100%;
                filter: opacity(0.5);
                background-color: #ffffff;
                padding: 0.5rem;
                border: 0;
                border-radius: 3px;
                margin-bottom: 1rem;
            }
        }
    }
}

@media screen and (max-width: 1215px) {
    .newsletter-centered{
        width: 95% !important;
    }
}
</style>