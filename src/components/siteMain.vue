<template>
    <div class="main-container">
        <hero />
        <cards1 />
    </div>
</template>

<script>
import hero from './hero.vue'
import cards1 from './cards-1.vue'
export default {
    name: "siteMain",

    components:{
        hero,
        cards1,
    }
};
</script>

<style>
</style>