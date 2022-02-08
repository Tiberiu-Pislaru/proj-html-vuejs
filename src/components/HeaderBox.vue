<template>
    <header>
        <div class="container">
            <div class="container-top">
                <div class="logo">
                    <img src="/images/logo_seo_w_1x.png" alt="">
                </div>

                <div class="top-right">

                    <nav>
                        <ul>
                            <li>
                                Home
                            </li>
                            <li>
                                Who We Are
                            </li>
                            <li>
                                What We Do
                            </li>
                            <li>
                                Where we work
                            </li>
                            <li>
                                Carrers
                            </li>
                            <li>
                                News
                            </li>
                            
                        </ul>
                    </nav>
                    <button class="button color-gs">
                        GET IN TOUCH NOW
                    </button>
                </div>

            </div>
            <div class="container-bottom">
                <h1>
                    SEM Campaigns Made Simple With Avada
                </h1>
                <p>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Maiores voluptatibus aliquam necessitatibus corporis soluta molestias asperiores minus sint accusantium in suscipit.
                </p>
                <div class="buttons">
                    <button class=" n-one button color-gs">
                        BUY AVADA NOW
                    </button>
                    <button class="button color-contact">
                        CONTACT US
                    </button>
                </div>
            </div>
        </div>
    </header>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
@import '@/style/variables.scss';
@import '@/style/utility.scss';

header{
    color: $color-white;
    background: url('/images/1-hero-image.png') no-repeat;
    background-position: center;
    background-size:cover;
    padding-top: 30px;

    .container{
        width: $width-container;
        margin:0 auto;

        .container-top{
            display: flex;
            justify-content: space-between;
            .top-right{
                display: flex;
                justify-content: space-between;
                flex-grow: 0.5;
                nav{
                    display: flex;
                    align-items: center;
                    flex-grow: 1;
                    ul{
                        
                        display: flex;
                        text-align:end;
                        justify-content: space-around;
                        list-style: none;
                        width: 100%;
                    }
                }
                
                
            }
                
        }

        .container-bottom{
            width: 50%;
            padding: 150px 0;

            h1{
                font-weight: bold;
                font-size:xxx-large;
            }

            p{
                margin: 15px 0; 
                padding-right: 85px;   
            }
            .n-one{
                margin-right: 15px;
            }
        }
        
    }
}

</style>