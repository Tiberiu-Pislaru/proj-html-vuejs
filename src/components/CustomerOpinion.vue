<template>
    <div class="container">
        <div class="title">
            <h1>
                What Our Clients Say
            </h1>
        </div>
        <card-customer :customer="datiClienti[currentIndex]"/>
        <indicators-image @mostra="showElement" :elements="datiClienti" :currentElement="currentIndex" />
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
        datiClienti:Array
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
}
</style>