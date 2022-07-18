<template>
    <section class="business">
        <div class="container">
            <div class="card">
                <span>OUR BUSINESS AREAS</span>
                <h2>Logistics Services</h2>
                <p>We are leaders in providing logistics service with a set of cuttig edge tecnologies and a team of experienced and renowned professionals </p>
                <span class="tag">Traditional</span>
                <span class="tag">Quality</span>
                <span class="tag">Security</span><br>
                <div class="btn">
                    <a href="#">READ MORE</a>
                </div>
                
            </div>

            <div class="card bg-white">
                <div class="mini-card">
                    <img src="../assets/img/gallery-3.jpg" alt="Technology">
                    <h3>Technology</h3>
                    <p>Focus on developing tecnology solution adapted to our client's need.</p>
                </div>
                
            </div>

            <div class="card bg-white">
                <div class="mini-card">
                    <img src="../assets/img/gallery-5.jpg" alt="Transport">
                    <h3>Transport</h3>
                    <p>We develop operational strategies to improve logistical efficency.</p>
                </div>
                
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name:"MainBusiness"

}
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';
@import '../assets/style/common.scss';
.business{
    width: 100%;
    background-color: $color_9;

    .container{
    width: 60%;
    margin: 0 auto;
    display: flex;
    justify-content: center;
    padding-block: 50px;

        .bg-white{
            background-color: $color_1;
        }

        .card{
            width: calc((100% / 3) - 20px);
            padding-inline: 20px;
            padding-bottom: 0;
            margin-right:15px;
            border-radius: 10px;
            

            span{
                color: $color_4;
                font-size: 12px;
                font-weight: bolder;
                display: inline-block;
            }

            h2{
                color: $color_10;
                font-size: 40px;
                line-height: 40px;
                padding-block: 15px;
            }

            p{
                font-size: 15px;
                padding-block: 15px;
                color: $color_5;
            }

            .tag{
                background-color: rgba($color: $color_12, $alpha: 0.5);
                margin-right: 5px;
                font-size: 12px;
                font-weight: 100;
                padding: 5px;
                display: inline-block;
                margin-bottom: 20px;
            }

            .btn{
                color: $color_1;
                background-color:$color_4;
                text-align: center;
                font-size: 13px;
                border-radius: 5px;
                padding: 5px;
                width: 40%;
            }
            
            .mini-card{
                width: 80%;
                margin: 0 auto;
                padding-top: 20px;
                
                h3{
                    padding-top: 20px;
                    color: $color_10;
                }

                p{
                    padding-bottom: 10px;
                }
            }

        }
    }
}



</style>>
