<template>
  <div id="app">
    <header-box :links='headerLinks'/> 
    <main-information-box/>
    <service-box/>
    <our-work-box/>
    <plans-box :plans="listPlans"/>
    <news-box/>
    <customer-box :customerData="customerData" :imgPartner="clientsPartner"/>
    <consultation-box/>
    <footer-box :footerLinks='footerLinks' :footerSocial='footerSocial'/> 
  </div>
</template>

<script>
import HeaderBox from "@/components/HeaderBox.vue"
import FooterBox from "@/components/FooterBox.vue"
import ConsultationBox from "@/components/ConsultationBox.vue"
import MainInformationBox from "@/components/MainInformationBox.vue"
import ServiceBox from "@/components/ServiceBox.vue"
import OurWorkBox from './components/OurWorkBox.vue'
import PlansBox from './components/PlansBox.vue'
import NewsBox from './components/NewsBox.vue'
import CustomerBox from './components/CustomerBox.vue'


export default {
  name: 'App',
  components: {
    HeaderBox,
    FooterBox,
    ConsultationBox,
    MainInformationBox,
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
          link:'#',
          open:true
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
      ],
      listPlans:[
        {
          name:'Standard',
          price:'19',
          numProjects:'5',
          storage:'5',
          users:'Unlimited'
        },
        {
          name:'Premium',
          price:'29',
          numProjects:'10',
          storage:'15',
          users:'Unlimited'
        },
        {
          name:'Professional',
          price:'39',
          numProjects:'15',
          storage:'30',
          users:'Unlimited'
        },
        {
          name:'Extreme',
          price:'59',
          numProjects:'Unlimited',
          storage:'Unlimited',
          users:'Unlimited'
        },
      ]
    }
  }
}
</script>

<style lang="scss">
@import './style/main.scss';

</style>
