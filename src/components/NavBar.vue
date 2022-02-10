<template>

    <div class="link">
        <a :href="data.link">{{data.name}}</a> 
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

    a{
        color:$color-white;
    }
    &:hover a{
        color:$yellow-orange;
    }
}
    

</style>