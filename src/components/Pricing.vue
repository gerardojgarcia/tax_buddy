<script>
import PricingCard from './PricingCard.vue';
export default {
    name: "Pricing",
   props: {
        price: String,
        type: String,
        use: String,
        features: Array,

    },
    components: { PricingCard }
}
</script>

<template>

<div>

    <h1>Simple pricing for everyone.</h1>

    <p>It doesn't matter what size your business is, our software will work well for you. </p>


</div>

<div class="pricing-info " >


            <PricingCard price="15" type="Small Business" use="Perfect for small / medium sized businesses." features="` [
              'Send 25 quotes and invoices',
              'Connect up to 5 bank accounts',
              'Track up to 50 expenses per month',
              'Automated payroll support',
              'Export up to 12 reports',
              'Bulk reconcile transactions',
              'Track in multiple currencies'
              ] `" />




</div>







</template>