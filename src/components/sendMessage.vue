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

<style>

</style>