<template>
    <div class="hero-container">
        <div class="hero-video">
            <video autoplay loop muted>
                <source src="../assets/video/city.mp4" type="video/mp4">
            </video>
        </div>
        <div class="hero-content">
            <div class="title">
                <h1>Lead</h1>
                <h1 class="space">~</h1>
                <div class="customer-container">
                    <div class="customer-bg"></div>
                    <h1>Customer</h1>
                </div>
            </div>
            <div class="text">
                <p>Succesful strategies require data analysis, creatifity and customer focus, taking 
                    advantage of the latest technologies to offer excellent services.</p>   
            </div>   
            <div class="hero-buttons-container">
                <button class="btn">GET IN TOUCH</button>
                <button class="btn border">READ MORE</button>    
            </div> 
        </div>
    </div>
</template>

<script>
export default {
    name : 'hero',

}
</script>

<style lang="scss">
@import '../assets/scss/common.scss';

.hero-container{
    height: calc(100vh - 30px);
    display: flex;
    justify-content: center;
    position: relative;
    overflow: hidden;

    .hero-video{
        position: absolute;
        filter: brightness(0.4);
        height: 100%;
        width: 100%;
        
        video{
            object-fit: cover;
            object-position: bottom;
            max-height: 100%;
            min-width: 100%
        }
    }

    .hero-content{
        position: absolute;
        top: 35%;
        display: flex;
        flex-direction: column;
        align-items: center;
        font-size: large;
        width: 60%;
        height: 30%;

        .title{
            display: flex;
            position: relative;
            color: #ffffff;
            font-weight: 900;
            font-size: xx-large;
            
            .space{
                margin-left:1rem;
                margin-right: 0.5rem;
            }

            .customer-container{
                position: relative;
                h1{
                    padding: 0 0.5rem;
                }

                .customer-bg{
                    position: absolute;
                    background-color: $site_green;
                    height: 100%;
                    width: 100%;
                    filter: opacity(0.1);
                    text-align: center;
                }
            }
        }

        .text{
            text-align: center;
            color: #a2adae;
            margin-top: 2rem;
            font-size: x-large;
            font-weight: 900;
        }

        .hero-buttons-container{
            height: 50px;
            margin-top: 2rem;

            .btn{
                margin: 0 1rem;
            }

            .border{
                border: 2px solid $site_green !important;
                background-color: transparent !important;

                &:hover{
                    background-color: $site_green !important;
                }
            }
        }
    }
}

@media screen and (max-width: 1215px) {
    video{
        height: 100vh;
        width: 100vw !important;
    }

    .hero-content{
        width: 100% !important;
    }
}
</style>