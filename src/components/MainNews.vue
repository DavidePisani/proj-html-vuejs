<template>
    <section>
        <div class="container">
            <p>OUR EDITORIAL CONTENT</p>
            <span>Latest</span><span class="next">News</span>
            <div class="description">
                <p class="text">Every week we publish content about what is beast in the business world</p>
               <span><a class="btn" href="#">SEE ALL</a></span> 
            </div>

            <div class="card-cont">
                <div class="card">
                    <img src="../assets/img/news-1.jpg" alt="">
                    <div class="img-text">Increasing creativity is possible for everyone</div>
                </div>

                <div class="card">
                    <img src="../assets/img/news-2.jpg" alt="">
                    <div class="img-text">Because market reserch is part of the business plan</div>
                </div>

                <div class="card">
                    <img src="../assets/img/news-3.jpg" alt="">
                    <div class="img-text">Working from home is now a trand</div>
                </div>


            </div>


        </div>
    </section>
  
</template>

<script>
export default {
    nome:"MainNews"

}
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';
@import '../assets/style/common.scss';

    .container{
        width: 57%;
        margin: 0 auto;
        padding-block: 80px;

        p{
            color: $color_4;
            font-size: 12px;
            padding-bottom: 20px;
            font-weight: bolder;
        }

        span{
            color: $color_10;
            font-size: 40px;
            font-weight: bolder;
            padding-right: 10px;
        }

        .next{
            padding: 0 10px;
            color: $color_4;
            background-color: rgba($color: $color_4, $alpha: 0.3);
            border-radius: 3px;
        }

        .description{
            display: flex;
            justify-content: space-between;

            .text{
                font-size: 15px;
                padding-top: 20px;
                color: $color_5;
            }

            .btn{
                color: $color_1;
                background-color:$color_4;
                font-size: 13px;
                border-radius: 5px;
                padding: 8px 20px;
                
            }
        }

        .card-cont{
                display: flex;
                padding-top: 20px;
                
                .card{
                    width: calc(33.3333333333% - 20px);
                    margin: 10px;
                    position: relative;
                    

                    img{
                        border-radius: 10px;
                        filter: brightness(60%); 
                    }

                    .img-text{
                        width: 75%;
                        margin: 0 auto;
                        position: absolute;
                        bottom: 40px;
                        right: 13%;
                        color: #edf4ec;
                        font-size: 18px;
                        text-align: center;
                        font-weight: bolder;
                    }
                    

                   
                }
            }
    }

</style>