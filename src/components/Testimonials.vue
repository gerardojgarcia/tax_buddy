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

<div class=" flex flex-col text-left py-16 lg:items-center">
    <div class=" lg:flex lg:flex-col lg:justify-center lg:items-center pb-16">
        <h6 class="text-4xl mt-8 mx-4 lg:text-5xl lg:ml-16 lg:text-center">Loved by businesses worldwide</h6>
    
        <p class=" pt-4 mx-4 text-lg lg:ml-16 lg:text-lg lg:text-center lg:w-2/4 text-gray-600 ">Our software is so simple that can't help but fall in love with it. Simpliciyt is easy whe nyou just skip tons of mission-critical featuers.</p>
    
    
    
    
    
    </div>
    
    <div class="w-full flex flex-col md:flex-row md:w-5/6 md:flex-wrap md:mx-16 justify-center items-center">
        <div class="testimonial-cards m-4 md:flex-row  md:w-1/4 md:mx-8" v-for="testimonial in testimonials" :key="testimonial.id">
        
        
            <TestimonialsCard :testimonial="testimonial"/>
        
        
        
        
        
        </div>
    </div>
</div>




</template>