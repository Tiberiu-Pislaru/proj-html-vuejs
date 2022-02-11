<template>

    <div class="link">
        <a :href="data.link">{{data.name}}</a>
        <div class="apply" v-if="data.open !== undefined && data.open!==false"> Apply</div>
    </div>
    
</template>

<script>
export default {
    props:{
        data:Object,
    }
}
</script>

<style lang="scss" scoped>
@import '@/style/utility.scss';
@import '@/style/variables.scss';

    
.link{
    display: flex;
    align-items: center;
    a{
        color:$color-white;
    }
    &:hover a{
        color:$yellow-orange;
    }
    .apply{
        color:$yellow-orange;
        padding: 5px 10px;
        margin-left: 5px;
        border: 1px solid $yellow-orange;
        border-radius: 5px;
    }
}
    

</style>