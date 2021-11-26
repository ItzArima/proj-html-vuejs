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

<style>

</style>