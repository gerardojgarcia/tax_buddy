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
    <div class="container w-full px-4 flex flex-row flex-wrap ">
            <div class="trusted-cards w-full flex flex-row flex-wrap items-center" >
            
            <div class="trusted-card  w-2/4 m-0 flex-row flex-wrap  " v-for="partner in partners" :key="partner.id">
                <TrustedCard :partner="partner"/>
            </div>
            
            </div>
    </div>
</template>