<script>


    import HeroButtons from './HeroButtons.vue';


export default {
    name: 'Hero',

    components: {
        HeroButtons,
    }

}
</script>

<template>
    <div class="w-full flex flex-col items-center ">

            <h1 class="text-5xl font-bold mt-8 py-8 px-16 w-full">Accounting <span class="text-blue-700">made simple</span> for small businesses.</h1>

            <p class="px-4"> Most bookkeeping software is acurate, but hard to use. We make the opposite trade-off, and hope you don't get audited.</p>

        
    </div>

    <div class="my-16">
    
       <HeroButtons/>
    
    
    </div>
</template>