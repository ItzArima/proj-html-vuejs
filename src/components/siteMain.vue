<template>
    <div class="main-container">
        <hero />
        <cards1 />
        <aboutNetwork />
        <businessArea />
        <pricing />
        <news />
        <newsletter />
    </div>
</template>

<script>
import hero from './hero.vue'
import cards1 from './cards-1.vue'
import aboutNetwork from './aboutNetwork.vue'
import businessArea from './businessArea.vue'
import pricing from './pricing.vue'
import news from './news.vue'
import newsletter from './newsletter.vue'

export default {
    name: "siteMain",

    components:{
        hero,
        cards1,
        aboutNetwork,
        businessArea,
        pricing,
        news,
        newsletter
    }
};
</script>

<style>
</style>