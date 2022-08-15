<script>
export default {
    name: 'Simplify',
}
</script>

<template>



    <div class="w-full flex flex-col bg-blue-300">
        <div class="flex flex-col px-4 py-4 bg-white">
            <h4 class="text-4xl text-left mt-16">Simplify Everyday business tasks.</h4>
            <p class="text-left py-4">Because you'd probably be a little confused if we suggested you complicate your
                everyday business tasks instead</p>
        </div>

        <div class="simplify-card bg-gray-200 flex flex-col pb-8 ">
             


            <div class="text-left w-full px-4 isolate shadow bg-white rounded pb-10 pt-8">

               <div class="self-start  text-4xl   bg-white rounded ">
                    <div class="bg-blue-500 w-16 h-16 flex flex-col justify-center rounded-lg items-center">
                    
                    <i class="fa-solid fa-chart-line text-white  "></i>
                    
                    </div>


                </div>


                <p class="text-blue-600 py-4">Reporting</p>
                <strong class="text-2xl font-normal my-4">Stay on top of things with always up-to-date reporting features. </strong>

                <p class="py-4 text-gray-500">We talked about reporting the stection above but we needed three tiems
                    here, so metnioning it one more time for posterity.</p>

            </div>

            <div class="w-full shadow-lg z-2 translate-x-4  -translate-y-4">

                <img src="/reporting.png" alt="" class="rounded">


            </div>


        </div>
        <div class="simplify-card bg-gray-200 pb-8">

           

            <div class="text-left w-full px-4 isolate shadow bg-white rounded pb-10 pt-8">
            <div class="self-start  text-4xl   bg-white rounded ">
                    <div class="bg-blue-500 w-16 h-16 flex flex-col justify-center rounded-lg items-center">
                    
                    <i class="fa-solid fa-bars-staggered text-white  "></i>
                    
                    </div>


                </div>
                <p class="text-blue-600  py-4">Inventory</p>
                <strong class="text-2xl font-normal my-4">Never lose track of what's in stock with acfurate inventory tracking. </strong>

                <p class="py-4 text-gray-500">We don't offer this as part of our software but that statement is naarguyably true. Accurate inventory tracking would help you for sure. </p>

            </div>

            <div class="w-full shadow-lg z-2 translate-x-4  -translate-y-4">

                <img src="/inventory.png" alt="" class="rounded">


            </div>


        </div>
        <div class="simplify-card bg-gray-200  pb-8">

         

            <div class="text-left w-full px-4 isolate shadow bg-white rounded pb-10 pt-8">
            <div class="self-start  text-4xl   bg-white rounded ">
                    <div class="bg-blue-500 w-16 h-16 flex flex-col justify-center rounded-lg items-center">
                    
                    <i class="fa-solid fa-users text-white  "></i>
                    
                    </div>


                </div>
                <p class="text-blue-600 py-4">Contacts</p>
                <strong class="text-2xl font-normal my-4">Organize all of your contacts, service, providers, and invoices in one place.  </strong>

                <p class="py-4 text-gray-500 ">This also isn't actually a feature, it's just some friendly advice. We definitely recommend that you do this. You'll feel really organized and pofessional.</p>

            </div>

            <div class="w-full shadow-lg z-2 translate-x-4  -translate-y-4">

                <img src="/contacts.png" alt="" class="rounded">


            </div>


        </div>
    </div>


</template>


<style scoped>
img {
    height: 500px;
    min-width: 800px;


}
</style>
