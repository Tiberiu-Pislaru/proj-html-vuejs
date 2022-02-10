<template>
    <div class="card">
        <div class="img">
            <img :src="`${customer.image}`" alt="">
        </div>
        <div class="opinion">
            {{customer.opinion}}
        </div>

        <div class="other">

            <div class="name">
                {{customer.name}},
            </div>
            <div class="startup">
                {{customer.startup}}
            </div>

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
        img{
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
    }
    .opinion {
        margin: 15px 0;
    }
    .other{
        display: flex;
        width: fit-content;
        margin: 0 auto;
        align-items:baseline;
        .name{
            font-size:20px;
            font-weight:bold;
            margin-right: 10px;
        }
    }
}
</style>