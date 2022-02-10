<template>
  <div id="app">
    <header-box :data='headerLinks'/> 
    <main-information/>
    <service-box/>
    <our-work-box/>
    <plans-box/>
    <news-box/>
    <customer-box :datiClienti="customerData" :imgPartner="clientsPartner"/>
    <consultation-box/>
    <footer-box :footerLinks='footerLinks' :footSocial='footerSocial'/> 
  </div>
</template>

<script>
import HeaderBox from "@/components/HeaderBox.vue"
import FooterBox from "@/components/FooterBox.vue"
import ConsultationBox from "@/components/ConsultationBox.vue"
import MainInformation from "@/components/MainInformation.vue"
import ServiceBox from "@/components/ServiceBox.vue"
import OurWorkBox from './components/OurWorkBox.vue'
import PlansBox from './components/PlansBox.vue'
import NewsBox from './components/NewsBox.vue'
import CustomerBox from './components/CustomerOpinion.vue'


export default {
  name: 'App',
  components: {
    HeaderBox,
    FooterBox,
    ConsultationBox,
    MainInformation,
    ServiceBox,
    OurWorkBox,
    PlansBox,
    NewsBox,
    CustomerBox
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
      ],
      customerData:[
        {
          image:'/images/testimonials-2.jpg',
          opinion:'GOOD!!!',
          name:'Luis Desalvo',
          startup:'CREO TECH'
        },
        {
          image:'/images/testimonials-1.jpg',
          opinion:'GOOD!!!',
          name:'Luisa Desalvo',
          startup:'CREO TECH'
        },
      ],
      clientsPartner:[
        '/images/clients_partner_6-200x202.png',
        '/images/clients_partner_5-200x202.png',
        '/images/clients_partner_1-200x202.png',
        '/images/clients_partner_2-200x202.png',
      ]
    }
  }
}
</script>

<style lang="scss">
@import './style/main.scss';

</style>
