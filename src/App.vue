  <script >
import Header from './components/Header.vue';
import Nav from './components/Nav.vue';
import HeaderButton from './components/HeaderButton.vue';
import Hero from './components/Hero.vue'
import Trusted from './components/Trusted.vue'
import TrustedCard from './components/TrustedCard.vue'
import Features from './components/Features.vue'
import Simplify from './components/Simplify.vue';
import CallToAction from './components/CallToAction.vue';
import Testimonials from './components/Testimonials.vue';
import TestimonialsCard from './components/Testimonials.vue';
import Pricing from './components/Pricing.vue';

export default {
  components: {
    Header,
    Nav,
    HeaderButton,
    Hero,
    Trusted,
    TrustedCard,
    Features,
    Simplify,
    CallToAction,
    Testimonials,
    TestimonialsCard,
    Pricing
},


  data() { 
    
    
    
    
    return {

      partners: [],
      testimonials:[],
      pricing: [],


    }

    },


    created() { 

     this.partners = [ 
      {
          id: 1,
          name: 'Statamic',
          src: '/statamic.png'


        },
        {
          id: 2,
          name: 'StaticKit',
          src: '/statickit.png'


        },
        {
          id: 3,
          name: 'Transistor',
          src: '/transistor.png'


        },
        {
          id: 4,
          name: 'Laravel',
          src: '/laravel.png'


        },
        {
          id: 5,
          name: 'Mirage',
          src: '/mirage.png'


        },
        {
          id: 6,
          name: 'Tuple',
          src: '/tuple.png'


        }
        
        ],

        this.testimonials = [
          {
            id:1,
            name: 'Sheryl Berge',
            position: 'Ceo at Lynch LLC',
            description: "TaxBuddy is so easy to use I can't help but wonder it it's realy doing the things the government expects me to do."

          },
           {
            id:2,
            name: 'Amy Hahn',
            position: 'Director at Veolocity Industries',
            description: "I'm trying to get a hold of someone in support, I'm in al ot of trouble right now and they are saying it has soemthing to do ith my books. Please get back to me right away."

          },
           {
            id:3,
            name: 'Leland Kiehn',
            position: 'Founder of Kiehn and Sons',
            description: "The best part about TaxBuddy is eveyr time I pay my employees, my bank balance doesn't go down like it used to. Looking forward to spending this etra cash when i figure out why my card is being declineed."

          },
           {
            id:4,
            name: 'Erin Powlowski',
            position: 'COO at Armstrong Inc',
            description: "There are so many things I had to do with my old software that I just don't do at all with TaxBuddy. Suspicious but I can't say i don't love it. "

          }
        ],

       this.pricing = [
          {
            id:1,
            price: "15",
            type: "Small Business",
            use: "Perfect for small / medium sized businesses.",
            features: [
              'Send 25 quotes and invoices',
              'Connect up to 5 bank accounts',
              'Track up to 50 expenses per month',
              'Automated payroll support',
              'Export up to 12 reports',
              'Bulk reconcile transactions',
              'Track in multiple currencies'
              ]

           
          },
           {
            id:2,
            price: "9",
            type: "Starter",
            use: "Good for anyone who is self-employed and just getting started.",
            features: [
              'Send 10 quotes and invoices',
              'Connect up to 2 bank accounts',
              'Track up to 15 expenses per month',
              'Manual payroll support',
              'Export up to 3 reports',
              
              ]

           
          },
           {
            id:3,
            price: "39",
            type: "Enterprise",
            use: "For even the biggest enterprise companies.",
            features: [
              'Send unlimited quotes and invoices',
              'Connect up to 15 bank accounts',
              'Track up to 200 expenses per month',
              'Automated payroll support',
              'Export up to 25 reports, including TPS',
              ]

           
          }

       ]


    }
    
    
    
    
    
}



</script>

<template>
  
  <div>
  
    <Header/>
    <Hero />
    <Trusted :partners="partners"/>
    <Features/>
  <Simplify/>
  <CallToAction/>
  <Testimonials :testimonials="testimonials"/>
  <Pricing :pricing="pricing"/>
  
  
  </div>
</template>

<style scoped>

</style>
