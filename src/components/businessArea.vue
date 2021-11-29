<template>
    <div class="business-container">
        <div class="business-centered">
            <p class="green">OUR BUSINESS AREAS</p>
            <div class="business-title">
                <div class="title-left">
                    <h1>Excellence in</h1>
                </div>
                <div class="title-right">
                    <div class="title-bg"></div>
                    <h1 class="hidden">Services</h1>
                    <h1 class="absolute">Services</h1>
                </div>
            </div>
            <div class="business-text">
                <p>We are leaders in providing consultancy services with a set of cutting-edge technologies and a team of
                    experienced and renowned professionals. These are some options that you can hire.
                </p>
                <button class="btn">SEE ALL</button>
            </div>
            <div class="business-cards">
                <div class="row margin-bottom">
                    <div class="card">
                        <i class="fas fa-network-wired fa-2x"></i>
                        <h2>Audit & Assurance</h2>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                        <button class="btn">READ MORE</button>
                    </div>
                    <div class="card middle">
                        <i class="fas fa-briefcase fa-2x"></i>
                        <h2>Financial Advisory</h2>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                        <button class="btn">READ MORE</button>
                    </div>
                    <div class="card">
                        <i class="far fa-chart-bar fa-2x"></i>
                        <h2>Analytics and M&A</h2>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                        <button class="btn">READ MORE</button>
                    </div>
                </div>
                <div class="row">
                    <div class="card">
                        <i class="fas fa-plane fa-2x"></i>
                        <h2>Middle Marketing</h2>
                        <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit.</p>
                        <button class="btn">READ MORE</button>
                    </div>
                    <div class="card middle">
                        <i class="fas fa-globe-europe fa-2x"></i>
                        <h2>Legal Consulting</h2>
                        <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit.</p>
                        <button class="btn">READ MORE</button>
                    </div>
                    <div class="card">
                        <i class="fas fa-hdd fa-2x"></i>
                        <h2>Regulatory Risk</h2>
                        <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit.</p>
                        <button class="btn">READ MORE</button>
                    </div>
                </div>
            </div>
        </div>    
    </div>
</template>

<script>
export default {
    name : 'businessArea'
}
</script>

<style lang="scss">
@import '../assets/scss/common.scss';

.business-container{
    display: flex;
    justify-content: center;
    background-color: #121117;
    padding: 5rem 0;

    .business-centered{
        width: 75%;

        .green{
            color: $site_green;
            margin-bottom: 1rem;
        }

        .business-title{
            display: flex;
            margin-bottom: 2rem;

            h1{
                color: #ffffff;
            }

            .title-right{
                position: relative;
                padding: 0 0.5rem;
                
                .title-bg{
                    height: 100%;
                    width: 100%;
                    background-color: $site_green;
                    filter: opacity(0.3);
                }

                .hidden{
                    visibility: hidden;
                    position: relative;
                    top: 0;
                    padding: 0 0.5rem;
                }

                .absolute{
                    position: absolute;
                    top: 0;
                    padding-left: 0.5rem;
                }
            }
        }

        .business-text{
            display: flex;
            margin-bottom: 2rem;
            justify-content: space-between;
            
            p{
                width: 70%;
            }

            .btn{
                background-color: transparent !important;
                border: 2px solid $site_green !important;

                &:hover{
                    background-color: $site_green !important;
                }
            }
        }

        .business-cards{

            .margin-bottom{
                margin-bottom: 2rem;
            }

            .row{
                display: flex;

                .middle{
                    margin: 0 2rem;
                }

                .card{
                    width: calc(100% / 3);
                    background-color: #1e2223;
                    padding: 3rem;
                    border-radius: 7px;
                    position: relative;
                    transition: all 0.3s;
                    top: 0;

                    i{
                        color: $site_green;
                        margin-bottom: 1.5rem;
                        transition: all 0.5s;
                    }

                    h2{
                        margin-bottom: 1.5rem;
                    }

                    p{
                        margin-bottom: 1.5rem;
                    }

                    .btn{
                        background-color: transparent !important;
                        border: 2px solid $site_green !important;

                        &:hover{
                            background-color: $site_green !important;
                        }
                    }

                    &:hover{
                        top: -10px;

                        i{
                            color: #e3e7df;
                        }
                    }
                }
            }
        }
    }
}

@media screen and (max-width: 1215px) {
    .business-centered{
        width: 95% !important;

        .card{
            display: flex;
            flex-direction: column;
            justify-content: space-between;
        }
    }
}
</style>