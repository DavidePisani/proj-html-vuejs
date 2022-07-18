<template>
  <div id="app">
    <HeaderComponent :headerLinks="headerLinks"/>

    <main>
      <MainBusiness/>
      <MainCompany/>
      <MainPartner/>
      <MainNews/>
      <MainNewsLetter/>
    </main>

  </div>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue'
import MainBusiness from './components/MainBusiness.vue'
import MainCompany from './components/MainCompany.vue'
import MainPartner from './components/MainPartner.vue'
import MainNews from './components/MainNews.vue'
import MainNewsLetter from './components/MainNewsLetter.vue'

export default {
  name: 'App',
  components: {
    HeaderComponent,
    MainBusiness,
    MainCompany,
    MainPartner,
    MainNews,
    MainNewsLetter,

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
            element:[ "ciao", ],
            itemImg:"fa-chevron-right",
            url:"#"
            
          },
          {
            footerTitle:"About",
            element:[ "ciao", ],
            itemImg:"fa-chevron-right",
            url:"#"
            
          },
          {
            footerTitle:"About",
            element:[ "ciao", ],
            itemImg:"fa-chevron-right",
            url:"#"
            
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
