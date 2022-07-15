<template>
  <div id="app">
    <HeaderComponent :headerLinks="headerLinks"/>

    <main>

    </main>

  </div>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue'

export default {
  name: 'App',
  components: {
    HeaderComponent
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
            text: 'BLOGS',
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
