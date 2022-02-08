<template>
    <footer>

        <div class="container-footer">

            <div class="logo">
                <img src="/images/logo_seo_1x.png" alt="">
            </div>

            <div class="links">
                <ul>
                    <li v-for="(link,index) in footerLinks" :key="index">
                        <a :href="link.link">{{link.name}}</a>
                    </li>
                </ul>
            </div>

            <div class="credits">
                <ul>

                    <li class="border-right pd-ex">
                        &copy; Copyright 2021-2020
                    </li>

                    <li class="border-right pd-ex">
                        Avada Theme by <span>ThemeFusion</span>
                    </li>

                    <li class="border-right pd-ex">
                        All rights reserved
                    </li>

                    <li class="pd-ex">
                        Powered by <span>WordPress</span>
                    </li>

                </ul>
            </div>

            <div class="social">
                <span class="social-network" v-for="social in footSocial" :key="social"><font-awesome-icon :icon="['fab', social]"/></span>
            </div>

        </div>

    </footer>
</template>

<script>
export default {
    props: {
        footerLinks:Array,
        footSocial:Array,
    }
}
</script>

<style lang="scss" scoped>
@import '@/style/utility.scss';
@import '@/style/variables.scss';

footer{
    padding: 45px 0;
    .container-footer {
        width: calc(100%/2);
        margin: 0 auto;
        text-align: center;
        color: $color-black;
        .links {
            margin: 45px 0;
            a{
                color:$color-black;
            }
        }
        .credits{
            ul{
                justify-content: center;
                li{
                    font-size: 13px;
                    span{
                        font-weight:bold;
                    }
                }
            }
        }
        .social{
            margin-top:30px;
    
            .social-network {
                font-size: 30px;
            }
        }
    }
}
</style>