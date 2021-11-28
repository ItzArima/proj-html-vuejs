<template>
    <div class="main-container">
        <stickyHeader />
        <div class="site-content">
            <hero id="home"/>
            <cards1 />
            <aboutNetwork id="about"/>
            <businessArea id="services"/>
            <pricing id="pricing"/>
            <news id="blog"/>
            <newsletter />
            <message id="touch"/>
        </div>    
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
import message from './sendMessage.vue'
import stickyHeader from './stickyHeader.vue'

export default {
    name: "siteMain",

    components:{
        hero,
        cards1,
        aboutNetwork,
        businessArea,
        pricing,
        news,
        newsletter,
        message,
        stickyHeader
    },

};
</script>

<style lang="scss">
@import '../assets/scss/common.scss';

.main-container{
    color: #e3e7df;
    position: relative;

    .site-content{
        position: relative;
        top: -82px;
    }        
}
</style>