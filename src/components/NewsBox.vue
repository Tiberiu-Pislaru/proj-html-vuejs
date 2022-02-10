<template>
    <div class="container-se pd-tb">

        <div class="container-service">
            <div class="title">
                <h1>Our News</h1>
                <p>Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudatium.</p>
            </div>

            <div class="container-box">

                <div class="box">

                    <div class="img-box">
                        <img src="/images/related-service-2-700x441.jpg" alt="">
                    </div>

                    <h3>Why You Need A SEO Agency Now</h3>

                    <p class="date">November 1st, 2017</p>

                    <div class="body-news">
                        <p>Aliquam non elit lacus. Praesent aliquet, ipsum id scelerisque convallis, mi ligula euismod odio, vel dictum mi risus a mi.</p>
                    </div>

                </div>

                <div class="box">

                    <div class="img-box">
                        <img src="/images/related-service-4-700x441.jpg" alt="">
                    </div>

                    <h3>SEO Tips For Your Startup</h3>

                    <p class="date">November 1st, 2017</p>

                    <div class="body-news">
                        <p>Aliquam non elit lacus. Praesent aliquet, ipsum id scelerisque convallis, mi ligula euismod odio, vel dictum mi risus a mi.</p>
                    </div>

                </div>

                <div class="box">

                    <div class="img-box">
                        <img src="/images/blog-post-6-700x441.jpg" alt="">
                    </div>

                    <h3>Image Optimization For Your Site</h3>

                    <p class="date">November 1st, 2017</p>

                    <div class="body-news">
                        <p>Aliquam non elit lacus. Praesent aliquet, ipsum id scelerisque convallis, mi ligula euismod odio, vel dictum mi risus a mi.</p>
                    </div>

                </div>

            </div>
            <button class="button color-gs">GO TO NEWS</button>
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
    background: $concrete;
    .container-service{
        width:$width-container;
        margin: 0 auto;
        text-align: center;
        .title{
            width: 55%;
            margin: 0 auto;
            margin-bottom: 30px;
            p{
                padding:0 45px;
                padding-top: 30px;
            }
        }
        .container-box{
            display: flex;
            justify-content:space-around;
            .box{
                width:calc(100%/3 - 15px);
                padding: 30px 15px;

                .img-box{
                    width: 100%;
                    img{
                        width: 100%;

                    }
                }
                
                h3{
                    margin: 15px 0;
                    color: $yellow-orange;
                }
                .date{
                    margin: 15px 0;
                }
                .body-news p{
                    line-height: 25px;
                }
                
            }
        }
        button{
            color:$color-white;
        }
    }

}

</style>