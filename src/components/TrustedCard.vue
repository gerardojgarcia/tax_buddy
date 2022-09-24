<script>
export default {
    name: 'TrustedCard',


        props: {
            partner: Object,
            
        },
methods: {




    
    
},

}
</script>

<template>



    <div >

                <img :src="partner.src" :alt="partner.name">

            </div>







</template>


<style scoped>

   @media (min-width: 900px){

        img {
            width: 10rem;
            
        }


   }


</style>