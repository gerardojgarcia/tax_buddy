<script>
import PricingCardButton from "./PricingCardButton.vue";
export default {
    name: 'PricingCard',

    props: {
        price: String,
        type: String,
        use: String,
        features: Array,

    },

    components: {
    PricingCardButton
}
}
</script>

<template>

        <div class="w-full flex flex-col rounded-3xl bg-blue-600 text-left px-4 mt-16 pb-16 text-white lg:mx-16 lg:w-1/5 ">

               <div class="pt-12 lg:ml-8">
                   <strong class="text-5xl"> ${{price}}</strong>
                   
                    <p class="py-2 text-lg font-bold ">{{type}}</p>
                    <p class="py-1 text-md">{{use}}</p>
               </div>
<div class="self-center my-8">

        <PricingCardButton />
</div>

                <div class="flex flex-col   lg:w-full px-8" >
                    <p class="text-left "  > <i></i></p>
                </div>                







        
        
        
        
        </div>



</template>