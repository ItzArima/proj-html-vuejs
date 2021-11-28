<template>
  <div id="app">
    <siteHeader />
    <siteMain />
    <siteFooter :footerElements="this.footerData"/>
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
    },

    data(){
        return{
            footerData: [
                {
                    title: 'About',
                    links: [
                        {
                            name: 'The Company'
                        },
                        {
                            name: 'Institutional'
                        },
                        {
                            name: 'Social & Events'
                        },
                        {
                            name: 'Innovation'
                        },
                        {
                            name: 'Environment'
                        },
                        {
                            name: 'Technologyy'
                        },
                    ]
                },
                {
                    title: 'Services',
                    links: [
                        {
                            name: 'Audit & Assurance'
                        },
                        {
                            name: 'Financial Advisory'
                        },
                        {
                            name: 'Analytics M&A'
                        },
                        {
                            name: 'Middle Marketing'
                        },
                        {
                            name: 'Legal Consulting'
                        },
                        {
                            name: 'Regulatory Risk'
                        },
                    ]
                },
                {
                    title: 'Support',
                    links: [
                        {
                            name: 'Responsability'
                        },
                        {
                            name: 'Terms of use'
                        },
                        {
                            name: 'About Cookies'
                        },
                        {
                            name: 'Privacy Policy'
                        },
                        {
                            name: 'Accessibility'
                        },
                        {
                            name: 'Information'
                        },
                    ]
                },
            ]
        }
    }


}
</script>

<style lang="scss">
    @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@900&display=swap');
    @import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@300&display=swap');
</style>
