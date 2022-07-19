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
      // struttura dati per compilare l'header
        headerLinks:[
          {
            text: 'HOME',
            url: '#',
          },

          {
            text: 'SERVICE',
            url: '#service',
          },

          {
            text: 'SKILLS',
            url: '#skills',
          },

          {
            text: 'PARTNERS',
            url: '#partners',
          },

          {
            text: 'BLOG',
            url: '#blog',
          },
        ],
        // struttura dati per compilare il footer
        footerLinks:[
          {
            footerTitle:"About",
            element:[ "The Company","Institutional", "Social & Event", "Innovation", "Environment", "Technology" ],
            itemImg:"fa-solid fa-chevron-right",
            url:"#"
          },
          {
            footerTitle:"Transportr",
            element:[ "Industrial","Chemical", "Packaged", "Construction", "Laminated Wood", "And others" ],
            itemImg:"fa-solid fa-chevron-right",
            url:"#" 
          },
          {
            footerTitle:"Support",
            element:[ "Responsability","Terms of Use", "About Cookies", "Privacy Policy", "Accessibility", "Information" ],
            itemImg:"fa-solid fa-chevron-right",
            url:"#"
          },
            
        ]
    }
  }
}
</script>

<style lang="scss">
 @import './assets/style/common.scss';
</style>
