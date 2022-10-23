<script>

import PricingCardButton from "./PricingCardButton.vue";
export default {
    name: "Pricing",
   props: {
        price: String,
        type: String,
        use: String,



    },




    components: { 
        
        
        
        
        

      PricingCardButton
        
        
        
        }
}
</script>

<template>

<div class=" flex flex-col text-left lg:text-center bg-blue-900 pb-16">
    <div class="mx-4 pt-16 lg:my-16 ">
    
        <strong class="text-4xl lg:text-6xl text-white">Simple pricing for everyone.</strong>
    
        <p class="py-4 text-white">It doesn't matter what size your business is, our software will work well for you. </p>
    
    
    </div>

  <!--Pricing card container-->
    
    <div class="pricing-info flex flex-col lg:flex-row lg:self-center lg:justify-center lg:w-5/6" >



<!--Pricing Card-->
      <div class="w-full flex flex-col rounded-3xl bg-blue-600 text-left px-4 mt-16 pb-16 text-white md:bg-blue-900 lg:mx-16 lg:w-2/6 ">

        <div class="pt-12 px-4 lg:ml-8">
          <strong class="text-5xl"> $9</strong>

          <p class="py-4 text-lg font-bold ">Starter</p>
          <p class="py-1 text-md">Good for anyone who is self-employed and just getting started</p>
        </div>
        <div class="self-center my-8">

          <PricingCardButton />
        </div>

        <div class="flex flex-col lg:w-full px-8" >
          <!--Features list-->

          <p class="text-left py-2"  > <i class="fa-solid fa-check"></i> Send 25 quotes and invoices</p>
          <p class="text-left py-2"  > <i class="fa-solid fa-check"></i> Connect up to 5 banks</p>
          <p class="text-left py-2"  ><i class="fa-solid fa-check"></i>Track up to 50 expenses per month</p>
          <p class="text-left py-2"  > <i class="fa-solid fa-check"></i> Automated payroll support</p>
          <p class="text-left py-2"  > <i class="fa-solid fa-check"></i> Export up to 12 reports</p>
          <p class="text-left py-2"  > <i class="fa-solid fa-check"></i>BUlk reconcile transactions</p>
          <p class="text-left py-2"  > <i class="fa-solid fa-check"></i>Track in multiple currencies</p>

        </div>



      </div>
      <!--Pricing Card-->
      <div class="w-full flex flex-col rounded-3xl bg-blue-900 md:bg-blue-600 border-blue-600 text-left px-4 mt-16 pb-16 text-white lg:mx-16 lg:w-2/6 ">

        <div class="pt-12  px-4 lg:ml-8">
          <strong class="text-5xl"> $15</strong>

          <p class="py-4 text-lg font-bold ">Small Business</p>
          <p class="py-1 text-md">Perfect for small / medium sized businesses.</p>
        </div>
        <div class="self-center my-8">

          <PricingCardButton />
        </div>

        <div class="flex flex-col   lg:w-full px-4" >
          <!--Features list-->

          <p class="text-left py-2"  > <i class="fa-solid fa-check"></i> Send 25 quotes and invoices</p>
          <p class="text-left py-2"  > <i class="fa-solid fa-check"></i> Connect up to 5 banks</p>
          <p class="text-left py-2"  ><i class="fa-solid fa-check"></i>Track up to 50 expenses per month</p>
          <p class="text-left py-2"  > <i class="fa-solid fa-check"></i> Automated payroll support</p>
          <p class="text-left py-2"  > <i class="fa-solid fa-check"></i> Export up to 12 reports</p>
          <p class="text-left py-2"  > <i class="fa-solid fa-check"></i>BUlk reconcile transactions</p>
          <p class="text-left py-2"  > <i class="fa-solid fa-check"></i>Track in multiple currencies</p>
        </div>


      </div>
      <!--Pricing Card-->
      <div class="w-full flex flex-col rounded-3xl bg-blue-900 text-left px-4 mt-16 pb-16 text-white lg:mx-16 lg:w-2/6 ">

        <div class="pt-12 px-4  lg:ml-8">
          <strong class="text-5xl"> $39</strong>

          <p class="py-4 text-lg font-bold ">Enterprise</p>
          <p class="py-1 text-md">For even the biggest enterprise companies</p>
        </div>
        <div class="self-center my-8">

          <PricingCardButton />
        </div>

        <div class="flex flex-col   lg:w-full px-8" >
          <!--Features list-->

          <p class="text-left py-2"  > <i class="fa-solid fa-check"></i> Send 25 quotes and invoices</p>
          <p class="text-left py-2"  > <i class="fa-solid fa-check"></i> Connect up to 5 banks</p>
          <p class="text-left py-2"  ><i class="fa-solid fa-check"></i>Track up to 50 expenses per month</p>
          <p class="text-left py-2"  > <i class="fa-solid fa-check"></i> Automated payroll support</p>
          <p class="text-left py-2"  > <i class="fa-solid fa-check"></i> Export up to 12 reports</p>
          <p class="text-left py-2"  > <i class="fa-solid fa-check"></i>Bulk reconcile transactions</p>
          <p class="text-left py-2"  > <i class="fa-solid fa-check"></i>Track in multiple currencies</p>
        </div>



      </div>

    </div>
</div>







</template>

<style scoped>


i {
  margin-right: 2rem;
}


</style>