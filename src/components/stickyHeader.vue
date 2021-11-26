<template>
  <div class="stickyheader-container" :class="{nav_colored: scrollPosition > 200}">
    <div class="nav-container">
      <div class="nav-left">
        <div class="logo-container">
          <div class="left-logo">
            <div class="background-logo"></div>
            <h1>NEX</h1>
          </div>
          <div class="right-logo">
            <h1>GEN</h1>
          </div>
        </div>
      </div>
      <div class="nav-right">
        <a href="#">HOME</a>
        <a href="#">ABOUT</a>
        <a href="">SERVICES</a>
        <a href="">PRICING</a>
        <a href="">BLOG</a>
        <button class="btn">GET IN TOUCH</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "stickyHeader",
    data() {
        return{
            scrollPosition: null
        }
    },
    mounted() {
        window.addEventListener('scroll', this.updateScroll);
    },
    methods: {
        updateScroll() {
            this.scrollPosition = window.scrollY
        }
    }   
};
</script>

<style lang="scss">

</style>