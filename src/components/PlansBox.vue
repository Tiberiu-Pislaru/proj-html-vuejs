<template>
    <div class="container-se pd-tb">

        <div class="container-service">
            <div class="title">
                <h1>Our Plans</h1>
                <p>Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudatium.</p>
            </div>

            <div class="container-box">

                <div class="box" v-for="(plan, num) in listPlans" :key="num">
                    <card-plan :plan="plan"/>
                </div>

            </div>
        </div>
    </div>
</template>

<script>

import CardPlan from './CardPlan.vue'
export default {
    components: {
        CardPlan,
    },
    props:{
        listPlans:Array
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
                padding-top: 30px;
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