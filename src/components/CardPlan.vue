<template>
    <div class="card">


        <h2>{{plan.name}}</h2>

        <div class="price">
            <div class="dollar-icon"><font-awesome-icon icon="fa-solid fa-dollar-sign" /></div>
            <div class="num">
                {{plan.price}}<sup>99</sup>
                <div class="tag-month">
                    monthly
                </div>
            </div>
        </div>

        <div class="carat">
            {{plan.numProjects}} Projects
        </div>
        <div class="carat">
            {{plan.storage}} GB Storage
        </div>
        <div class="carat">
            {{plan.users}} Users
        </div>

        <button class="button">START TODAY</button>
    </div>
</template>

<script>
export default {
    props:{
        plan:Object,
    }
}
</script>

<style lang="scss" scoped>
@import '@/style/utility.scss';
@import '@/style/variables.scss';

.card{
    background-color: $color-white;
    padding: 30px 15px;
    .price{
        display: flex;
        justify-content: center;
        .num{
            font-size: 30px;
            color: aqua;
            font-weight: bold;
            position: relative;
            sup{
                font-size:18px;
            }
            .tag-month{
                position: absolute;
                color:#bcbbbc;
                font-size:10px;
                bottom: 0;
                right: -50%;
            }
        }
    }
    
    h2{
        margin-bottom: 30px ;
    }
    .carat{
        margin: 10px 0;
        color:grey;
    }
    .button{
        border: 2px solid grey;
        background-color: $color-white;
        transition: all .5s;
        &:hover{
            background-color: $yellow-orange;
            border-color:transparent;

        }
    }
}

</style>