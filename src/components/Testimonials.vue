<script>
import TestimonialsCard from './TestimonialsCard.vue';
export default {
    name: "Testimonials",
    components: { 
        
        TestimonialsCard,
        
        },
        props: {
            testimonials: Array
        }
}
</script>
<template>

<div class="text-left py-16 ">
    <div class="pb-16">
        <h6 class="text-4xl mt-8 mx-4">Loved by businesses worldwide</h6>
    
        <p class=" pt-4 mx-4 text-lg">Our software is so simple that can't help but fall in love with it. Simpliciyt is easy whe nyou just skip tons of mission-critical featuers.</p>
    
    
    
    
    
    </div>
    
    <div class="testimonial-cards w-full flex flex-col" v-for="testimonial in testimonials" :key="testimonial.id">
    
    
        <TestimonialsCard :testimonial="testimonial"/>
    
    
    
    
    
    </div>
</div>




</template>