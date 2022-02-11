<template>
    <div class="container-info">
        <div class="title">
            <h1>Meet The New Acency SEO Template From The Avada Team</h1>
            <p>Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudatium.</p>
        </div>

        <div class="container-box">

            <div class="box">

                <div class="icon">
                    <font-awesome-icon icon="fa-solid fa-road" />
                </div>

                <h2>Establish Goals</h2>

                <p>Aliquam non elit lacus. Praesent aliquet, ipsum id scelerisque convallis, mi ligula euismod odio, vel dictum mi risus a mi.</p>

            </div>

            <div class="box">

                <div class="icon">
                    <font-awesome-icon icon="fa-solid fa-video" />
                </div>

                <h2>Work With A Team</h2>

                <p>Aliquam non elit lacus. Praesent aliquet, ipsum id scelerisque convallis, mi ligula euismod odio, vel dictum mi risus a mi.</p>

            </div>

            <div class="box">

                <div class="icon">
                    <font-awesome-icon icon="fa-solid fa-droplet" />
                </div>

                <h2>Get Results</h2>

                <p>Aliquam non elit lacus. Praesent aliquet, ipsum id scelerisque convallis, mi ligula euismod odio, vel dictum mi risus a mi.</p>

            </div>


        </div>
        <div class="img">
            <img src="/images/agency-seo-desk-front.jpg" alt="">
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

.container-info{
    width:$width-container;
    margin: 0 auto;
    text-align: center;
    padding-top: 30px;
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
            width:calc(100%/3 - 30px);
            background-color: $concrete;
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

</style>