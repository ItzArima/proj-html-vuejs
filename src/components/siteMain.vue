<template>
    <div class="main-container">
        <hero />
        <cards1 />
        <aboutNetwork />
        <businessArea />
        <pricing />
    </div>
</template>

<script>
import hero from './hero.vue'
import cards1 from './cards-1.vue'
import aboutNetwork from './aboutNetwork.vue'
import businessArea from './businessArea.vue'
import Pricing from './pricing.vue'
export default {
    name: "siteMain",

    components:{
        hero,
        cards1,
        aboutNetwork,
        businessArea,
        Pricing
    }
};
</script>

<style>
</style>