<template>
    <section class="newsletter" id="blog">
        <div class="container">
            <div class="card">
                 <p class="about">NEWSLETTER</p>
                <span class="prev">Know</span><span>First</span>
                <div class="descriprion">Follow closely and recive content about our company and the nwes of the current company</div>
            </div>

            <div class="card">
                <input type="text" placeholder="Name"><br>
                <input type="email" placeholder="Email"><br>
                <a class="btn" href="#">SUBSCRIBE</a>
            </div>
        </div>

    </section>
  
</template>

<script>
export default {
    name:"MainNewsLetter"

}
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';
@import '../assets/style/common.scss';
.newsletter{
    background-image: url(../assets/img/bg-1.jpg);
    background-position: center;
    background-size: cover;
    width: 100%;

    .container{
        width: 50%;
        margin: 0 auto;
        padding-block: 110px;
        display: flex;

        .card{
            width: 50%;

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
                color:$color_1;
                font-size: 40px;
                font-weight: bolder;
                padding-left: 8px;
                padding-bottom: 10px;
            }
            .descriprion{
                font-size: 14px;
                padding-top: 25px;
                color: $color_5;
            }

            input{
                width: 90%;
                height: 40px;
                margin-bottom: 20px;
                outline: none;
                padding-left: 10px;
                border-radius:5px;
                border: 0;
                opacity: 0.5;
            }

            .btn{
                color: $color_1;
                background-color:$color_4;
                font-size: 13px;
                border-radius: 5px;
                padding: 8px 25px;
            }
        }
    }
}

</style>