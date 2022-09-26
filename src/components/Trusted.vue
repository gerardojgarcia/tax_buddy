<script>
import TrustedCard from './TrustedCard.vue'

export default {
    name: 'Trusted',

props: {
    partners: Array,
},

components: {
    TrustedCard,
}


}
</script>

<template>
    <div class=" w-full pt-16 px-4 flex flex-col flex-wrap ">
        <p class="text-lg self-center mt-16 mb-8">Trusted by these companies</p>
            <div class="trusted-cards w-full mb-16 md:w-3/5 md:m-auto flex flex-row flex-wrap justify-center items-center" >
            
            <div class="trusted-card  w-2/5 m-0 flex-row flex-wrap md:flex-nowrap md:w-1/6 md:mb-16" v-for="partner in partners" :key="partner.id">
                <TrustedCard :partner="partner"/>
            </div>
            
            </div>
    </div>
</template>

<style scoped>

   



</style>