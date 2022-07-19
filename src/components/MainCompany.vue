<template>
  <section class="company" id="skills">
    <div class="container-company">
        <div class="card">
            <p class="about">ABOUT THE NETWORK</p>
            <span class="prev">The</span><span>Company</span>
            <div class="descriprion">With all of the expertise and capabily comes an unrivalled commitment to customer service.</div>
            <!-- start -->
            <div class="mini-card">
                <div class="percent">
                    <div class="number">0</div>
                </div>

                <div class="text">
                    <h4>Leadership</h4>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. </p>
                </div>
            </div>
            <!-- end -->
            <!-- start -->
            <div class="mini-card">
                <div class="percent">
                    <div class="number">0</div>
                </div>

                <div class="text">
                    <h4>Psichology</h4>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. </p>
                </div>
            </div>
            <!-- end -->
            <!-- start -->
            <div class="mini-card">
                <div class="percent">
                    <div class="number">1</div>
                    <div class="bar"></div>
                </div>

                <div class="text">
                    <h4>Flexibility</h4>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. </p>
                </div>
            </div>
            <!-- end -->
        </div>
    </div>

    <div class="container-company">
        <img src="../assets/img/about-5.jpg" alt="">
        </div>
  </section>
</template>

<script>
export default {
name:"MainCompany"
}
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';
@import '../assets/style/common.scss';
.company{
    background-color: $color_2;
    width: 100%;
    display: flex;
    .container-company{
        width: 50%;
        display: flex;
        justify-content: flex-end;

        .card{
            color: $color_1;
            padding-top: 100px;
            width: 56%;

            .about{
                color: $color_4;
                font-size: 12px;
                padding-bottom: 20px;
                font-weight: bolder;
            }
            .prev{
                font-size: 40px;
                font-weight: bolder;
                padding: 0 10px;
                background-color: rgba($color: $color_4, $alpha: 0.3);
                border-radius: 3px;
            }
            span{
                font-size: 40px;
                font-weight: bolder;
                padding-left: 10px;
            }
            .descriprion{
                font-size: 15px;
                padding-block: 15px;
                color: $color_5;
            }

            .mini-card{
                display:flex;
                padding-top: 50px;

                .percent{
                    width: 90px;
                    height: 90px;
                    line-height: 75px;
                    border: 7px solid rgba($color: $color_3, $alpha: 0.3);
                    border-radius: 50%;
                    flex-shrink: 0;
                    position:relative;
                        .number{
                            text-align: center;
                            font-size: 30px;
                            &:after{
                            content:"%";
                            font-size: 10px;
                            }
                        } 

                        .bar{
                            position:absolute;
                            top:50%;
                            left: -7px;
                            width: 6px;
                            height: 2px;
                            background-color: $color_4;
                            border: 0;
                        }
                   
                }

                .text{
                    padding-left: 30px;

                    h4{
                        font-size: 20px;
                        color:$color_1 ;
                    }

                    p{
                        font-size: 15px;
                        padding-top: 15px;
                        color: $color_5;
                    }
                }
            }

        }
            
        
        
    }
        

    }
</style>