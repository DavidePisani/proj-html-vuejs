<template>
  <section class="partner">
    <div class="container">
        <ul>
            <li v-for="image , index in partnerImg" :key="index">
                <img :src="image.url" :alt="image.name">
            </li>

            
        </ul>
       
    </div>

  </section>
</template>

<script>
export default {
name:"MainPartner",
    data(){
        return{
            partnerImg:[
                {
                    url:require("../assets/img/logo-5.png"),
                    name:"less"
                },
                {
                    url:require("../assets/img/logo-1.png"),
                    name:"wooCommerce"
                },
                {
                    url:require("../assets/img/logo-2.png"),
                    name:"WordPress"
                },
                {
                    url:require("../assets/img/logo-3.png"),
                    name:"pingdom"
                },
                {
                    url:require("../assets/img/logo-4.png"),
                    name:"jquery"
                },
                {
                    url:require('../assets/img/logo-5.png'),
                    name:"less"
                },
                
            ]
        }
    }

}
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';
@import '../assets/style/common.scss';

.partner{
    width: 100%;
   background-color: $color_9;

   .container{
    width: 55%;
    margin: 0 auto;
    padding-block:50px;

        ul{
            display: flex;
            align-items: center;
        }

        li{
            list-style-type: none;
            padding: 35px;
            text-align: center;

            img{
               opacity: 0.5;
            }
            
        }
   }
}

</style>