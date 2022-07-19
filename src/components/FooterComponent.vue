<template>
  <footer>
    <div class="footer-top">
        <div class="container">
            <div class="card">
                <div class="name">
                    <span class="prev">NEX</span>
                    <span class="next">GEN</span>
                </div>
                <p>A Functional HTML Tempate for Corporate & Business </p>
                <span class="icon"><i class="fa-solid fa-phone"></i> +1(305)1234-5678 </span> 
                <span class="icon"><i class="fa-solid fa-envelope"></i> hello@example.com </span> 
                <span class="icon"><i class="fa-solid fa-location-dot"></i> Main Avenue, 987 </span> 
                <a class="btn-transp" href="#"> GET IN TOUCH</a>
            </div>
            <!-- genero 3 card con li -->
            <div v-for="element , index in footerLinks" :key="index" class="card bg-white">
                <ul>
                    <h4>{{element.footerTitle}}</h4>
                    <li v-for="links, index in element.element" :key="index">
                        <a :href='element.url'><i :class='element.itemImg'></i>
                        {{links}}
                        </a>
                    </li>
                </ul>
            </div>
        </div>
    </div>

    <div class="footer-bottom">
        <div class="container">
            <div class="text">
                Enjoi the low price. We are tracking any intention of piracy
            </div>

            <div class="text">
                <i class="fa-regular fa-copyright"></i>
                2020 NEGXGEN is Proudly Powered By
                <span>Codings</span>
            </div>
        </div>
    </div>
  </footer>
</template>

<script>
export default {
nome:"FooterComponent",
    props:{
        footerLinks: Array
    }

}

</script>


<style lang="scss" scoped>
@import '../assets/style/variables.scss';
@import '../assets/style/common.scss';
.footer-top{
    background-image: url(../assets/img/bg-10.jpg);
    background-position: center;
    background-size: cover;

    .container{
        width: 60%;
        margin: 0 auto;
        display: flex;
        padding-block: 130px;

        .bg-white{
            background-color: rgba($color: $color_9, $alpha: 0.1);
            border-radius: 10px;
           
            padding: 30px;
        }
        
        .card{
                width: calc(25% - 35px);
                margin-right: 25px;

            .name{
            color:$color_9;
            font-size: 18px;
            font-weight: bolder;
            letter-spacing: 3px;

                .prev{
                    color:#00a6a6;
                    background-color: rgba($color: $color_15, $alpha: 0.2);
                    padding: 7px 0px 7px 25px;
                    border-radius: 50px 0px 0px 50px;
                }
            }

            p{
                font-size: 14px;
                padding-block: 20px;
                color: $color_5;
            }

            .icon{
                display: block;
                padding-block: 5px;
                color: $color_5;
                font-size: 15px;
                
                i{
                    margin-right: 5px;
                }
            }

             .btn-transp{
                color: $color_1;
                border: 1px solid $color_4 ;
                font-size: 13px;
                border-radius: 5px;
                padding: 8px 20px;
                margin-top:20px
            }

            h4{
                color: $color_1;
                font-size: 18px;
                padding-bottom: 10px;
            }

            li{
                list-style-type: none;
                color: $color_5;
                padding-block: 2px;
                font-size: 14px;

                &:hover{
                   color: $color_4;
                }
            }

        }       
    }
}

.footer-bottom{
    background-color: $color_2;
    width: 100%;
    .container{
        width: 60%;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        padding-top:30px;
        padding-bottom:3px;

        .text{
            color:$color_5;
            font-size: 13px;

            span{
                color: $color_15;
            }

            i{
                height: 100%;
                font-size: 10px; 
                vertical-align: -webkit-baseline-middle;
            }
        }
    }
}

</style>