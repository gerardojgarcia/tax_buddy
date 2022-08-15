  <script >
import Header from './components/Header.vue';
import Nav from './components/Nav.vue';
import HeaderButton from './components/HeaderButton.vue';
import Hero from './components/Hero.vue'
import Trusted from './components/Trusted.vue'
import TrustedCard from './components/TrustedCard.vue'
import Features from './components/Features.vue'
import Simplify from './components/Simplify.vue';

export default {
  components: {
    Header,
    Nav,
    HeaderButton,
    Hero,
    Trusted,
    TrustedCard,
    Features,
    Simplify
},


  data() { 
    
    
    
    
    return {

      partners: [],

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
  
  
  </div>
</template>

<style scoped>

</style>
