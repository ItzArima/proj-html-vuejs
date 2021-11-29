<template>
    <div class="header-container">
        <div class="info-contacts-container">
            <div class="left-contacts">
              <i class="fas fa-clock"></i>
              <p>Open Hour: Mon - Sat - 9:00 - 18:00</p>
            </div>
            <div class="right-contacts">
                <div class="phone-number">
                    <i class="fas fa-phone-alt"></i>
                    <p>+1 (305) 1234-5678</p>
                </div>
                <div class="mail-contact">
                    <i class="fas fa-envelope"></i>
                    <p>Hello@example.com</p>
                </div>
                <div class="social-pages">
                    <i class="fab fa-facebook-f"></i>
                    <i class="fab fa-twitter"></i>
                    <i class="fab fa-linkedin-in"></i>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name:'siteHeader',
}
</script>

<style lang="scss">
@import '../assets/scss/common.scss';

.header-container{
    background-color: $site_green;
    color: #e3e7df;
    height: 50px;
    line-height: 50px;
    display: flex;
    justify-content: center;
    
    .info-contacts-container{
        display: flex;
        justify-content: space-between;
        align-items: center;
        width: 75%;

        .left-contacts{
            display: flex;
            align-items: center;
        }

        .right-contacts{
            display: flex;

            div{
                display: flex;
                align-items: center;
                margin: 0 1rem;
            }

            .social-pages{
                margin-right: 0;
                
                i{
                    margin: 0 1rem;
                }
            }
        }

        i{
            margin: 0 0.5rem;
        }
    }
}

@media screen and (max-width: 1215px) {

}
</style>