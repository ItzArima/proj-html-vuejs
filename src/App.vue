<template>
  <div id="app">
    <siteHeader />
    <siteMain />
    <siteFooter />
  </div>
</template>

<script>
import siteHeader from './components/siteHeader.vue'
import siteMain from './components/siteMain.vue'
import siteFooter from './components/siteFooter.vue'

export default {
  name: 'App',
  components: {
    siteHeader,
    siteMain,
    siteFooter
  }
}
</script>

<style lang="scss">
    @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@900&display=swap');
    @import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@300&display=swap');
</style>
