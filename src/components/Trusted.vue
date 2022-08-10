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
    <div class="container w-full pt-16 px-4 flex flex-col flex-wrap ">
        <p class="text-lg self-center ">Trusted by these companies</p>
            <div class="trusted-cards w-full flex flex-row flex-wrap items-center" >
            
            <div class="trusted-card  w-2/4 m-0 flex-row flex-wrap  " v-for="partner in partners" :key="partner.id">
                <TrustedCard :partner="partner"/>
            </div>
            
            </div>
    </div>
</template>