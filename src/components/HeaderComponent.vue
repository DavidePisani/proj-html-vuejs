<template>
  <header>
    <div class="container header-top">
        <!-- orario e giorni di lavoro -->
        <div class="time-work">
            <i class="fa-solid fa-clock"></i>
            Open Hours: Mon-Sat-9.00 - 18.00
        </div>

        <!-- tutti i contatti -->
        <div class="contact">
            <div class="phone">
                <i class="fa-solid fa-phone"></i>
                +1(305)1234-5678
            </div>
            <div class="email">
                <i class="fa-solid fa-envelope"></i>
                hello@example.com
            </div>
            <div class="social">
                <a href="#"><i class="fa-brands fa-facebook-f"></i></a>
                <a href="#"><i class="fa-brands fa-twitter"></i></a>
                <a href="#"><i class="fa-brands fa-linkedin-in"></i></a>
            </div>
            
        </div>
    </div>
    <!-- Jumbotron -->
    <div class="jumbo">
        <!-- wrapper per oscurare un po l'immagine -->
        <div class="wrapper">
            <div class="container">
                <!-- nav bar  -->
                <div class="name">
                    <span class="prev">NEX</span>
                    <span>GEN</span>
                </div>

                <div class="nav-links">
                    <ul>
                        <li v-for="links,index in headerLinks " :key="index">
                        <a href="#">{{links.text}}</a> 
                        </li>

                        <li>
                            <a class="btn" href="#">GET IN THOUCH </a>
                        </li>
                    </ul>
                </div>
            </div>
            <!-- info jumbotron -->
            <div class="container right-info">
                <div class="info-jumbo">
                    <h1>Logistic that goes further.</h1>
                    <p>For 20 years working with the most innovative in the field of transport</p>
                    <a class="btn" href="#"> GET IN THOUCH</a>
                    <a class="btn-transp" href="#">READ MORE</a>
                </div>
                
            </div>
        </div>
    </div>
    
  </header>

</template>

<script>


export default {
    name:"HeaderComponent",

    props:{
        headerLinks: Array
    }
        
}
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';
 @import '../assets/style/common.scss';
    header{
        background-color: #21333e;
        .header-top{
            color: $color_9;
            height: 50px;
            line-height: 50px;
        }
        
        
        .container{
            width: 60%;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;

            .time-work{
               font-size: 12px;
            }

            .contact{
                font-size: 12px;
                display: flex;
                
                div{
                    padding-right: 25px;
                }

                .social i{
                    padding-right: 25px;
                }
            }
        }

        .jumbo{
            background-image: url(../assets/img/jumbo.jpg);
            width: 100%;
            height: 600px;
            background-position: center;
            background-size: cover;
            

            .wrapper{
                width: 100%;
                height: 100%;
                background-color: rgba($color: #000000, $alpha: 0.5);
                
                    .name{
                        color:$color_9;
                        padding-top: 15px;
                        font-size: 18px;
                        font-weight: bolder;

                        .prev{
                            color:$color_15;
                            background-color: rgba($color: $color_4, $alpha: 0.2);
                            padding: 7px;
                            border-radius: 50px 0px 0px 50px;
                        }
                    }

                    .nav-links {
                        padding-top: 15px;
                        ul{
                            display: flex;

                            li{
                                padding-right: 25px;
                                list-style-type: none;
                                color: $color_9;
                                font-size: 13px;
                                font-weight: 500;


                                .btn{
                                    color: inherit;
                                    background-color:$color_4;
                                    font-size: 13px;
                                    border-radius: 5px;
                                    padding: 8px 20px;
                                }
                            }
                        }
                    }
                    .right-info{
                        position: relative;
                        
                        .info-jumbo{
                            width: 30%;
                            position: absolute;
                            top: 90px;
                            left: 550px;

                        h1{
                            color: $color_1;
                            font-size: 60px;
                            font-weight: 700px;
                            padding-bottom: 20px;
                            line-height: 60px;
                            text-shadow: 1px $color_4 ;
                        }

                        p{
                            color:$color_5;
                            padding-bottom: 20px;
                            font-size: 17px;
                        }

                        .btn{
                            color: $color_1;
                            background-color:$color_4;
                            font-size: 13px;
                            border-radius: 5px;
                            padding: 8px 20px;
                            margin-right: 10px;
                        }

                        .btn-transp{
                            color: $color_1;
                            border: 1px solid $color_4 ;
                            font-size: 13px;
                            border-radius: 5px;
                            padding: 8px 20px;
                        
                        }
                    }

                }
                
            }  
        }
    }
</style>