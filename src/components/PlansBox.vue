<template>
    <div class="container-se pd-tb">

        <div class="container-service">
            <div class="title">
                <h1>Our Plans</h1>
                <p>Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudatium.</p>
            </div>

            <div class="container-box">

                <div class="box" v-for="num in 4" :key="num">
                    <card-plan/>
                </div>
                <!-- <div class="box">


                    <h2>Premium</h2>

                    <div class="price">
                        <div class="dollar-icon"><font-awesome-icon icon="fa-solid fa-dollar-sign" /></div>
                        <div class="num">
                            29<sup>99</sup>
                            <div class="tag-month">
                                monthly
                            </div>
                        </div>
                    </div>

                    <div class="carat">
                        10 Projects
                    </div>
                    <div class="carat">
                        15 GB Storage
                    </div>
                    <div class="carat">
                        Unlimited Users
                    </div>

                    <button class="button">START TODAY</button>
                </div>
                <div class="box">


                    <h2>Professional</h2>

                    <div class="price">
                        <div class="dollar-icon"><font-awesome-icon icon="fa-solid fa-dollar-sign" /></div>
                        <div class="num">
                            39<sup>99</sup>
                            <div class="tag-month">
                                monthly
                            </div>
                        </div>
                    </div>

                    <div class="carat">
                        15 Projects
                    </div>
                    <div class="carat">
                        30 GB Storage
                    </div>
                    <div class="carat">
                        Unlimited Users
                    </div>

                    <button class="button">START TODAY</button>
                </div>
                <div class="box">


                    <h2>Extreme</h2>

                    <div class="price">
                        <div class="dollar-icon"><font-awesome-icon icon="fa-solid fa-dollar-sign" /></div>
                        <div class="num">
                            59<sup>99</sup>
                            <div class="tag-month">
                                monthly
                            </div>
                        </div>
                    </div>

                    <div class="carat">
                        Unlimited Projects
                    </div>
                    <div class="carat">
                        Unlimited Storage
                    </div>
                    <div class="carat">
                        Unlimited Users
                    </div>

                    <button class="button">START TODAY</button>
                </div> -->

            </div>
        </div>
    </div>
</template>

<script>

import CardPlan from './CardPlan.vue'
export default {
    components: {
        CardPlan,
    }
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