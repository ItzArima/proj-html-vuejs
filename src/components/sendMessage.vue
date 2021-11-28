<template>
    <div class="message-container">
        <div class="message-centered">
            <div class="message-left">
                <p class="green">SEND MESSAGE</p>
                <div class="message-title">
                    <div class="title-left">
                        <h1>Get in</h1>
                    </div>
                    <div class="title-right">
                        <div class="title-bg"></div>
                        <h1 class="hidden">Touch</h1>
                        <h1 class="absolute">Touch</h1>
                    </div>
                </div>
                <div class="message-text">
                    <p>We will respond to your message as soon as possible.</p>
                </div>
                <div class="message-form">
                    <form action="#">
                        <div class="iconed">
                            <input name="name" type="text" placeholder="Name">
                            <img src="../assets/img/image-1.png" alt="">
                        </div>
                        <input name="mail" type="email" placeholder="Email">
                        <input name="phone" type="text" placeholder="Phone">
                        <div class="iconed">
                            <input name="more" type="text" placeholder="More info">
                            <i class="fas fa-angle-down"></i>
                        </div>    
                        <input class="message" name="message" type="text" placeholder="Message">
                        <button class="btn">SEND</button>
                    </form>
                </div>
            </div>
            <div class="message-right">
                <h3>Example Inc.</h3>
                <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit.</p>
                <p>Consectetur vel sint quam. Itaque, voluptatum quod.</p>
                <div class="contacts-container">
                    <div class="contact">
                        <div class="icon">
                            <div class="icon-bg"></div>
                            <i class="fas fa-phone-alt fa-lg"></i>
                        </div>   
                        <p>+1 (305) 1234-5678</p>
                    </div>
                    <div class="contact">
                        <div class="icon">
                            <div class="icon-bg"></div>
                            <i class="fas fa-envelope fa-lg"></i>
                        </div>   
                        <p>Hello@example.com</p>
                    </div>
                    <div class="contact">
                        <div class="icon">
                            <div class="icon-bg"></div>
                            <i class="fas fa-map-marker-alt fa-lg"></i>
                        </div>    
                        <p>Main Avenue, 987</p>
                    </div>
                    <button class="btn">VIEW MAP</button>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name : 'message'
}
</script>

<style lang="scss">
@import '../assets/scss/common.scss';

.message-container{
    display: flex;
    justify-content: center;
    padding: 7rem 0;

    .message-centered{
        width: 75%;
        display: flex;

        .message-left{
            width: 70%;
            
            .green{
                color: $site_green;
                margin-bottom: 1rem;
            }

            .message-title{
                display: flex;
                margin-bottom: 2rem;

                .title-left{
                    color: $site_black;
                }

                .title-right{
                    position: relative;

                    .title-bg{
                        background-color: $site_green;
                        filter: opacity(0.3);
                        height: 100%;
                        width: 100%;
                    }

                    .absolute{
                        position: absolute;
                        top: 0;
                        color: $site_green;
                        padding-left: 0.5rem;
                    }

                    .hidden{
                        visibility: hidden;
                        padding: 0 0.5rem;
                    }
                }
            }

            .message-text{
                
                p{
                    color: $site_black;
                    margin-bottom: 2rem;
                }
            }

            .message-form{

                form{
                    display: flex;
                    flex-wrap: wrap;
                    justify-content: space-between;

                    input{
                        width: 49%;
                        padding: 0.5rem;
                        background-color: #e3e7df;
                        border: 0;
                        margin-bottom: 1rem;
                        border-radius: 3px;
                    }

                    .iconed{
                        position: relative;
                        width: 49%;
                        display: flex;
                        align-items: center;
                        margin-bottom: 1rem;

                        input{
                            width: 100%;
                            margin-bottom: 0;
                        }

                        img{
                            position: absolute;
                            right: 0;
                            padding: 0.25rem;
                        }

                        i{
                            position: absolute;
                            right: 2%;
                            align-self: center;
                            color: $site_black;
                            filter: opacity(0.5);
                        }
                    }

                    .message{
                        width: 100%;
                        padding-bottom: 5rem;
                    }
                }
            }
        }

        .message-right{
            width: 30%;
            padding-left: 1.5rem;
            display: flex;
            flex-direction: column;
            justify-content: center;

            h3,p{
                color: $site_black;
                margin-bottom: 1rem;
            }

            .contacts-container{
                width: 100%;

                .contact{
                    display: flex;
                    width: 100%;
                    align-items: center;
                    margin-bottom: 1rem;

                    p{
                        margin-bottom: 0;
                    }

                    .icon{
                        position: relative;
                        display: flex;
                        justify-content: center;
                        align-items: center;
                        margin-right: 0.5rem;

                        .icon-bg{
                            height: 50px;
                            width: 50px;
                            background-color: $site_green;
                            filter: opacity(0.3);
                            text-align: center;
                            line-height: 50px;
                            border-radius: 50%;
                            position: relative;
                        }

                        i{
                            color: $site_green;
                            z-index: 2;
                            position: absolute;
                        }
                    }    
                }
            }

            .btn{
                background-color: transparent !important;
                border: 2px solid $site_green !important;
                margin-top: 1rem;
                color: $site_green;

                &:hover{
                    background-color: $site_green !important;
                    color: white;
                }
            }
        }
    }
}
</style>