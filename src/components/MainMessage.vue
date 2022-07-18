<template>
<section >
    <div class="container">
        <div class="card">
            <p class="about">SAND A MESSAGE</p>
            <span>Get In</span><span class="next">Touch</span>
            <div class="descriprion">We will respnde to your message as soon as possible</div>
            <form>
                <input type="text" placeholder="Name">
                <input type="email"  placeholder="Email"><br>
                <input type="number"  placeholder="Number">
                <select name="info" id="info" >
                    <option value="info">More Info</option>
                </select><br>
                <textarea name="message" id="message" cols="30" rows="10" placeholder="Message"></textarea>
            </form>
            <a class="btn" href="#">SEND</a>
        </div>

        <div class="info">
            <h4>Example inc.</h4>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
            <p>Present diam lacus, depibus sed imperdiet consectetur.</p>
            <span><i class="fa-solid fa-phone"></i> +1(305)1234-5678 </span> 
            <span><i class="fa-solid fa-envelope"></i> hello@example.com </span> 
            <span><i class="fa-solid fa-location-dot"></i> Main Avenue, 987 </span> 
            <a class="btn-transp" href="#"> VIEW MAP</a>
        </div>
    </div>

    
</section>
  
</template>

<script>
export default {
    name:"MainMessage"

}
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';
@import '../assets/style/common.scss';
section{
    width: 100%;
    background-color: $color_1;

    .container{
    width: 60%;
    margin: 0 auto;
    padding-block: 100px;
    display: flex;

        .card{
            width: 60%;
                .about{
                    color: $color_4;
                    font-size: 12px;
                    padding-bottom: 20px;
                    font-weight: bolder;
                }
                span{
                    font-size: 40px;
                    font-weight: bolder;
                    color: $color_10;
                    padding-right: 5px;
                }

                .next{
                    padding: 0 10px;
                    color: $color_4;
                    background-color: rgba($color: $color_4, $alpha: 0.3);
                    border-radius: 3px;
                }
            
                .descriprion{
                    font-size: 15px;
                    padding-block: 30px;
                    color: $color_5;
                }

                form{
                    
                    input{
                        width: 48%;
                        height: 30px;
                        margin-right: 10px;
                        margin-bottom: 10px;
                        border: none;
                        outline: none;
                        color: $color_5;
                        padding-left: 10px;
                        background-color: #dce2db;
                        border-radius: 5px;
                    }

                    select{
                        width: 48%;
                        height: 30px;
                        color: $color_5;
                        padding-left: 10px;
                        border: none;
                        outline: none;
                        background-color: #dce2db;
                        border-radius: 5px;
                    }

                    textarea{
                        width: 98%;
                        height: 125px;
                        color: $color_5;
                        outline: none;
                        padding:10px;
                        background-color: #dce2db;
                        border: none;
                        resize: none;
                        border-radius: 5px;
                    }
                    
                }
                .btn{
                    color: $color_1;
                    background-color:$color_4;
                    font-size: 13px;
                    border-radius: 5px;
                    padding: 8px 25px;
                    margin-top: 20px;
                }
        }

        .info{
            width: 39%;
            margin: 0 auto;
            padding-left: 20px;

                h4{
                color: $color_10;
                font-size: 20px;
                }
                p{
                    font-size: 15px;
                    padding-block: 15px;
                    color: $color_5;
                }
                span{
                    display: block;
                    padding-block: 10px;
                    color: $color_4;

                    i{
                        background-color:#cce3de;
                        width: 35px;
                        height: 35px;
                        border-radius: 35px;
                        text-align: center;
                        line-height: 35px;
                        margin-right: 10px;

                    }
                }
                .btn-transp{
                    color: $color_4;
                    border: 1px solid $color_4 ;
                    font-size: 13px;
                    border-radius: 5px;
                    padding: 8px 20px;
                    margin-top: 5px;   
                }
        }
    
    }

}


</style>