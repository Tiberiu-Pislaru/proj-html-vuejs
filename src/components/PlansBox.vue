<template>
    <div class="container-se pd-tb">

        <div class="container-service">
            <div class="title">
                <h1>Our Plans</h1>
                <p>Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudatium.</p>
            </div>

            <div class="container-box">

                <div class="box">


                    <h2>Standard</h2>

                    <div class="price">

                    </div>

                    <p>Aliquam non elit lacus. Praesent aliquet, ipsum id scelerisque convallis, mi ligula euismod odio, vel dictum mi risus a mi.</p>

                    <div class="link"><a href="#">Read More </a></div>
                </div>

            </div>
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
@import '@/style/utility.scss';
@import '@/style/variables.scss';

.container-se{
    background-image: url('/images/background1.jpg') ;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    background-color: $deep-cove;
  

    .container-service{
        width:$width-container;
        margin: 0 auto;
        text-align: center;
        .title{
            width: 55%;
            margin: 0 auto;
            margin-bottom: 30px;
            p{
                padding: 0 45px;
            }
        }
        .container-box{
            display: flex;
            justify-content:space-around;
            margin:60px 0;
            .box{
                width:calc(100%/4 - 15px);
                background-color: $color-white;
                padding: 30px 15px;
               
                h2{
                    margin-bottom: 30px ;
                }
                p{
                    line-height:25px
                }
                .link {
                    margin: 15px 0;
                    a{

                        color: $yellow-orange;
                    }

                }
            }
        }
        .img{
            width: 100%;
            display: flex;
            img{
                width: 100%;
            }
        }
    }

}

</style>