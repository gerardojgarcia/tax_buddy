<script>
export default {
    name: 'Simplify',

  methods: {
        simplifySelect(){

          const simplifyCardLg = document.getElementById('simplify-card-contact')
          const simplifyIcon = document.getElementById('simplify-icon')

           simplifyCardLg.classList.toggle('simplify-selected')
          simplifyIcon.classList.toggle('simplify-bg')

        }





  }

}
</script>

<template>



    <div class="w-full flex flex-col bg-white-300">
        <div class="flex flex-col px-4 py-4 bg-white md:self-center">
            <h4 class="text-3xl w-3/4 font-bold text-left mt-16 md:text-5xl md:font-normal md:text-center md:w-full md:mt-16">Simplify everyday business tasks.</h4>
            <p class="text-left text-lg py-4 md:w-3/4 md:text-center md:self-center">Because you'd probably be a little confused if we suggested you complicate your everyday business tasks instead</p>
        </div>

      <div class="md:hidden">
        <div class="simplify-card bg-gray-200 flex flex-col pb-8 ">
             


            <div class="text-left w-full px-4 isolate shadow bg-white rounded pb-10 pt-10">

               <div class="self-start  text-4xl   bg-white rounded ">
                    <div class="bg-blue-500 w-10 h-10 flex flex-col justify-center rounded-lg items-center">
                    
                    <i class="fa-solid fa-chart-line text-white text-base "></i>
                    
                    </div>


                </div>


                <p class="text-blue-600 pt-8 pb-4">Reporting</p>
                <strong class="text-2xl font-normal my-4">Stay on top of things with always up-to-date reporting features. </strong>

                <p class="py-4 text-gray-500">We talked about reporting the section above but we needed three times
                    here, so mentioning it one more time for posterity.</p>

            </div>

            <div class="w-full shadow-lg z-2 translate-x-4  -translate-y-4">

                <img src="/reporting.png" alt="" class="rounded">


            </div>


        </div >
        <div class="simplify-card bg-gray-200 pb-8">

           

            <div class="text-left w-full px-4 isolate shadow bg-white rounded pb-10 pt-10">
            <div class="self-start  text-4xl   bg-white rounded ">
                    <div class="bg-blue-500 w-10 h-10 flex flex-col justify-center rounded-lg items-center">
                    
                    <i class="fa-solid fa-bars-staggered text-white text-base "></i>
                    
                    </div>


                </div>
                <p class="text-blue-600  pt-8 pb-4">Inventory</p>
                <strong class="text-2xl font-normal my-4">Never lose track of what's in stock with acfurate inventory tracking. </strong>

                <p class="py-4 text-gray-500">We don't offer this as part of our software but that statement is naarguyably true. Accurate inventory tracking would help you for sure. </p>

            </div>

            <div class="w-full shadow-lg z-2 translate-x-4  -translate-y-4">

                <img src="/inventory.png" alt="Image of sample inventory" class="rounded">


            </div>


        </div>
        <div class="simplify-card bg-gray-200  pb-8">

         

              <div class="text-left w-full px-4 isolate shadow bg-white rounded pb-10 pt-10">
                <div class="self-start  text-4xl   bg-white rounded ">
                    <div class="bg-blue-500 w-10 h-10 flex flex-col justify-center rounded-lg items-center">
                    
                    <i class="fa-solid fa-users text-white text-base  "></i>
                    
                    </div>


                </div>
                <p class="text-blue-600 pt-8 pb-4">Contacts</p>
                <strong class="text-2xl font-normal my-4">Organize all of your contacts, service, providers, and invoices in one place.  </strong>

                <p class="py-4 text-gray-500 ">This also isn't actually a feature, it's just some friendly advice. We definitely recommend that you do this. You'll feel really organized and professional.</p>

            </div>

            <div class="w-full shadow-lg z-2 translate-x-4  -translate-y-4">

                <img src="/contacts.png" alt="" class="rounded">


            </div>


        </div>



      </div>

      <!--Simplify Categories Large Screen Layout-->
      <div class="simplify-categories-lg hidden md:flex w-5/6 isolate  md:px-36  md:flex-col md:bg-white self-center md:mt-10">

        <!--Simplify Card Lg flex  container-->
        <div class="flex flex-row overflow-x-auto  ">
        <!--Simplify Card Lg-->
        <div @click="simplifySelect()" id="simplify-card-contact" class="simplify-contact-lg mx-6 cursor-pointer simplify-selected">
          <div class="text-left w-full px-4 isolate  bg-white rounded pb-10 pt-10">
            <div class="self-start  text-4xl   bg-white rounded ">
              <div id="simplify-icon" class=" simplify-bg bg-gray-300 w-10 h-10 flex flex-col justify-center rounded-lg items-center">

                <i  class=" fa-solid fa-users text-white text-base  "></i>

              </div>


            </div>
            <p class="text-gray-400 pt-8 pb-4">Contacts</p>
            <strong class="text-xl font-normal my-4">Organize all of your contacts, service, providers, and invoices in one place.  </strong>

            <p class="py-4 text-gray-500 ">This also isn't actually a feature, it's just some friendly advice. We definitely recommend that you do this. You'll feel really organized and professional.</p>

          </div>

        </div>

        <!--Simplify Card Lg-->
        <div id="simplify-card-inventory" class="simplify-contact-lg px-6 cursor-pointer">
          <div class="text-left w-full px-4 isolate  bg-white rounded pb-10 pt-10">
            <div class="self-start  text-4xl   bg-white rounded ">
              <div class="bg-gray-300 w-10 h-10 flex flex-col justify-center rounded-lg items-center">

                <i class="fa-solid fa-users text-white text-base  "></i>

              </div>


            </div>
            <p class="text-gray-400  pt-8 pb-4">Inventory</p>
            <strong class="text-xl font-normal my-4">Organize all of your contacts, service, providers, and invoices in one place.  </strong>

            <p class="  py-4 text-gray-500 ">This also isn't actually a feature, it's just some friendly advice. We definitely recommend that you do this. You'll feel really organized and professional.</p>

          </div>

        </div>

        <!--Simplify Card Lg-->
        <div id="simplify-card-reporting" class="simplify-contact-lg px-6 cursor-pointer">
          <div class="text-left w-full px-4 isolate  bg-white rounded pb-10 pt-10">
            <div class="self-start  text-4xl   bg-white rounded ">
              <div class="bg-gray-300 w-10 h-10 flex flex-col justify-center rounded-lg items-center card-desc">

                <i class="fa-solid fa-users text-white text-base  "></i>

              </div>


            </div>
            <p class="text-gray-400 pt-8 pb-4">Reporting</p>
            <strong class="text-xl font-normal my-4">Organize all of your contacts, service, providers, and invoices in one place.  </strong>

            <p class="py-4 text-gray-500 ">This also isn't actually a feature, it's just some friendly advice. We definitely recommend that you do this. You'll feel really organized and professional.</p>

          </div>

        </div>
        </div>

        <!-- Simplify Lg image container-->

        <div class=" simplify-large-img-container flex flex-row bg-gray-200 mt-16 p-20 mb-24 overflow-x-auto no-scrollbar isolate rounded-3xl  self-center border-gray-800 shadow-inner">
          <div class="w-full shadow-lg z-2 mr-6 ">

            <img src="/contacts.png" alt="" class="rounded">


          </div>
          <div class="w-full shadow-lg z-2 ">

            <img src="/contacts.png" alt="" class="rounded">


          </div>
          <div class="w-full shadow-lg z-2 rounded-lg">

            <img src="/contacts.png" alt="" class="rounded">


          </div>


        </div>




      </div>


    </div>


</template>


<style scoped>
img {
    height: 500px;
    min-width: 800px;


}

.simplify-large-img-container {
  width: 65vw;
}

.simplify-large-img-container>.img{
  width: 100%;
  height: 300px;
}

.simplify-contact-lg:hover .card-desc {

  color: dodgerblue;

}

.simplify-selected {
  color: #535bf2;
}

.simplify-bg {
  background-color: #535bf2;

}

.no-scrollbar::-webkit-scrollbar {
  display: none;
}


</style>
