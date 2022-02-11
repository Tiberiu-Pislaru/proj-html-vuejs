<template>

    <div class="link">
        <a :href="link.link">{{link.name}}</a>
        <div class="apply" v-if="link.open !== undefined && link.open!==false"> Apply</div>
    </div>
    
</template>

<script>
export default {
    props:{
        link:Object,
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
        transition: all .3s;
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