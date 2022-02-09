<template>
    <div class="card">
        <div class="img">
            <img :src="`${customer.image}`" alt="">
        </div>
        <div class="opinion">
            {{customer.opinion}}
        </div>
        <div class="name">
            {{customer.name}}
        </div>
        <div class="startup">
            {{customer.startup}}
        </div>

    </div>
</template>

<script>
export default {
    props: {
        customer:Object
    }
}
</script>

<style lang="scss" scoped>
.card {
    display: flex;
    flex-direction: column;
    .img{
        border-radius:50%;
        overflow: hidden;
        width: fit-content;
        margin: 0 auto;
    }
}
</style>