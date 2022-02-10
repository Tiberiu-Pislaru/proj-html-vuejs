<template>
    <div class="container-se pd-tb">

        <div class="container-service">
            <div class="title">
                <h1>See Our Top Notch Services</h1>
                <p>Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudatium.</p>
            </div>

            <div class="container-box">

                <div class="box">

                    <div class="icon">
                        <font-awesome-icon icon="fa-brands fa-google" />
                    </div>

                    <h2>Google SEO</h2>

                    <p>Aliquam non elit lacus. Praesent aliquet, ipsum id scelerisque convallis, mi ligula euismod odio, vel dictum mi risus a mi.</p>

                    <div class="link"><a href="#">Read More</a></div>
                </div>

                <div class="box">

                    <div class="icon">
                        <font-awesome-icon icon="fa-solid fa-gear" />
                    </div>

                    <h2>Brand Strategy</h2>

                    <p>Aliquam non elit lacus. Praesent aliquet, ipsum id scelerisque convallis, mi ligula euismod odio, vel dictum mi risus a mi.</p>

                    <div class="link"><a href="#">Read More</a></div>
                </div>

                <div class="box">

                    <div class="icon">
                        <font-awesome-icon icon="fa-solid fa-building" />
                    </div>

                    <h2>Local SEO</h2>

                    <p>Aliquam non elit lacus. Praesent aliquet, ipsum id scelerisque convallis, mi ligula euismod odio, vel dictum mi risus a mi.</p>
                    <div class="link"><a href="#">Read More</a></div>

                </div>

                <div class="box">

                    <div class="icon">
                        <font-awesome-icon icon="fa-solid fa-chart-column" />
                    </div>

                    <h2>SEO Analysis</h2>

                    <p>Aliquam non elit lacus. Praesent aliquet, ipsum id scelerisque convallis, mi ligula euismod odio, vel dictum mi risus a mi.</p>
                    <div class="link"><a href="#">Read More</a></div>

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
    color: $color-white;
    background-image: url('/images/pattern_background.png'), ;
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
                padding: 30px 45px;
            }
        }
        .container-box{
            display: flex;
            justify-content:space-around;
            
            .box{
                width:calc(100%/4 - 15px);
                background-color: $lucky-point;
                padding: 30px 15px;
                .icon{
                    color: $yellow-orange;
                    font-size: 30px;
                }
                h2{
                    margin: 30px 0;
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