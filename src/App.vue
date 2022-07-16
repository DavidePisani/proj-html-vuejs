<template>
  <div id="app">
    <HeaderComponent :headerLinks="headerLinks"/>

    <main>
      <MainBusiness/>
      <MainCompany/>
    </main>

  </div>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue'
import MainBusiness from './components/MainBusiness.vue'
import MainCompany from './components/MainCompany.vue'

export default {
  name: 'App',
  components: {
    HeaderComponent,
    MainBusiness,
    MainCompany
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
