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

<style>

</style>