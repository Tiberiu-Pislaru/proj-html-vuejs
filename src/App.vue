<template>
  <div id="app">
    <header-box :data='headerLinks'/> 
    <consultation-box/>
    <footer-box :footerLinks='footerLinks' :footSocial='footerSocial'/> 
  </div>
</template>

<script>
import HeaderBox from "@/components/HeaderBox.vue"
import FooterBox from "@/components/FooterBox.vue"
import ConsultationBox from "@/components/ConsultationBox.vue"


export default {
  name: 'App',
  components: {
    HeaderBox,
    FooterBox,
    ConsultationBox
    
  },
  data(){
    return{
      headerLinks:[
        {
          name:'Home',
          link:'#'
        },
        {
          name:'Who We Are',
          link:'#'
        },
        {
          name:'What We Do',
          link:'#'
        },
        {
          name:'Where we work',
          link:'#'
        },
        {
          name:'Carrers',
          link:'#'
        },
        {
          name:'News',
          link:'#'
        }
      ],

      footerLinks:[
        {
          name:'Home',
          link:'#'
        },
        {
          name:'Who We Are',
          link:'#'
        },
        {
          name:'What We Do',
          link:'#'
        },
        {
          name:'Where we work',
          link:'#'
        },
        {
          name:'Carrers',
          link:'#'
        },
        {
          name:'News',
          link:'#'
        },
        {
          name:'Get In Touch Now',
          link:'#'
        },
      ],
      footerSocial:[
        'facebook-f',
        'instagram',
        'twitter',
        'youtube',
      ]
    }
  }
}
</script>

<style lang="scss">
@import './style/main.scss';

</style>
