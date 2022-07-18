<template>
  <div id="app">
    <HeaderComponent :headerLinks="headerLinks"/>

    <main>
      <MainBusiness/>
      <MainCompany/>
      <MainPartner/>
      <MainNews/>
      <MainNewsLetter/>
      <MainMessage/>
    </main>

    <FooterComponent :footerLinks="footerLinks"/>

  </div>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue'
import MainBusiness from './components/MainBusiness.vue'
import MainCompany from './components/MainCompany.vue'
import MainPartner from './components/MainPartner.vue'
import MainNews from './components/MainNews.vue'
import MainNewsLetter from './components/MainNewsLetter.vue'
import MainMessage from './components/MainMessage.vue'
import FooterComponent from './components/FooterComponent.vue'

export default {
  name: 'App',
  components: {
    HeaderComponent,
    MainBusiness,
    MainCompany,
    MainPartner,
    MainNews,
    MainNewsLetter,
    MainMessage,
    FooterComponent,

  },

  data(){
    return{
        headerLinks:[
          {
            text: 'HOME',
            url: '#',
          },

          {
            text: 'SERVICE',
            url: '#',
          },

          {
            text: 'SKILLS',
            url: '#',
          },

          {
            text: 'PARTNERS',
            url: '#',
          },

          {
            text: 'BLOG',
            url: '#',
          },
        ],

        footerLinks:[
          {
            footerTitle:"About",
            element:[ "The Company","Institutional", "Social & Event", "Innovation", "Environment", "Technology" ],
            itemImg:"fa-solid fa-chevron-right",
          },
          {
            footerTitle:"Transportr",
            element:[ "Industrial","Chemical", "Packaged", "Construction", "Laminated Wood", "And others" ],
            itemImg:"fa-solid fa-chevron-right", 
          },
          {
            footerTitle:"Support",
            element:[ "Responsability","Terms of Use", "About Cookies", "Privacy Policy", "Accessibility", "Information" ],
            itemImg:"fa-solid fa-chevron-right",
          },
            
        ]
    }
  }
}
</script>

<style lang="scss">
 @import './assets/style/common.scss';
#app {


}
</style>
