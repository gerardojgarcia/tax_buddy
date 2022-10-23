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
    <div class="w-full flex flex-col items-center md:mt-16 ">

            <div class=" mt-16 py-8 px-4 w-full md:w-3/5">
                <h1 class="text-5xl md:text-7xl font-bold">Accounting <span class="text-blue-700">made simple</span> for small businesses.</h1>
            </div>

            <p class="px-4 text-lg"> Most bookkeeping software is accurate, but hard to use. We make the opposite trade-off, and hope you don't get audited.</p>

        
    </div>

    <div class="mt-10">
    
       <HeroButtons/>
    
    
    </div>
</template>