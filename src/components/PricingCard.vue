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

        <div class="w-full flex flex-col rounded-lg bg-blue-600 text-left px-4 mt-16 text-white">

               <div class="pt-8">
                   <strong class="text-4xl "> ${{price}}</strong>
                   
                    <p class="py-2 text-lg font-bold ">{{type}}</p>
                    <p class="py-1 text-md">{{use}}</p>
               </div>
<div class="self-center my-8">

        <PricingCardButton />
</div>

                <p> {{features}}</p>                







        
        
        
        
        </div>



</template>