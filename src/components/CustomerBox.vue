<template>
    <div class="container pd-tb">
        <div class="title">
            <h1>
                What Our Clients Say
            </h1>
        </div>
        <card-customer :customer="customerData[currentIndex]"/>
        <indicators-image @show="showElement" :elements="customerData" :currentElement="currentIndex" />
        <div class="container-imgs">
            <div class="img" v-for="(img,index) in imgPartner" :key="index">
                <img :src="`${img}`" alt="">
            </div>
        </div>
    </div>
</template>

<script>
import CardCustomer from './CustomerCard.vue'
import IndicatorsImage from './IndicatorsImage.vue'


export default {
    components: {
        CardCustomer,
        IndicatorsImage,
    },
    props: {
        customerData:Array,
        imgPartner:Array,
    },
    data() {
        return {
            currentIndex: 0
        };
    },
    methods: {
        showElement(elementIndex) {
            this.currentIndex = elementIndex;
        }
    }
}
</script>

<style lang="scss" scoped>
@import '@/style/utility.scss';
@import '@/style/variables.scss';
.container {
    width:$width-container;
    margin: 0 auto;
    text-align: center;
    .container-imgs {
        display: flex;
        justify-content: space-around;
        .img{
            width: calc(100%/7);
            img{
                width: 100%;
                object-fit: cover;
            }
        }
    }
}
</style>