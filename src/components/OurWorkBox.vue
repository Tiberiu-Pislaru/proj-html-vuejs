<template>
    <div class="container-w pd-tb">

        <div class="container-work">
            <div class="title">
                <h1>Our Work</h1>
                <p>Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudatium.</p>
            </div>

            <div class="container-box">

                <div class="box">
                    <img src="/images/case-study-gallery-3-1.jpg" alt="">
                </div>

                <div class="box">
                    <img src="/images/case-study-gallery-2.jpg" alt="">
                </div>

                <div class="box">
                    <img src="/images/case-study-gallery-1-1.jpg" alt="">
                </div>

                <div class="box">
                    <img src="/images/case-study-gallery-4-1.jpg" alt="">
                </div>

                <div class="box">
                    <img src="/images/case-study-gallery-5-1.jpg" alt="">
                </div>

                <div class="box">
                    <img src="/images/case-study-gallery-6-1.jpg" alt="">
                </div>
                
                <button class="button color-gs">VIEW OUR WORK</button>

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

.container-w{
    // color: $color-white;

    .container-work{
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
            flex-wrap: wrap;
            .box{
                width:calc(100%/3 - 15px);
                margin-bottom: 15px;
                display: flex;
                img{
                    width: 100%;
                    object-fit: contain;
                }
                
            }
            button{
                margin-top: 15px;
            }
        }
        
    }
}

</style>