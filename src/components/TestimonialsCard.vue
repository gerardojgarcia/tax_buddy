<script>
export default {
    name: 'TestimonialsCard',


    props: {
        testimonial: Object,
    }

}
</script>


<template>


    <div class="w-full mx-4 rounded-lg shadow-lg  mt-8 md:mx-16 flex flex-col md:flex-row md:flex-wrap text-left pb-4">
    
        <div class="mx-8 mt-4 card-description">
            <p class="description text-lg">{{testimonial.description}}</p>
        </div>
        <div class="flex flex-col mt-8 mb-4 mx-8">
            <strong class="name">{{testimonial.name}}</strong>
            <p class="text-sm text-gray-500 pt-1">{{testimonial.position}}</p>
        </div>

    
    </div>


</template>

<style scoped>



    .card-description {
        border-bottom: 1px solid rgba(128, 128, 128, 0.432);
        padding-bottom: 2rem; 
    }


    



</style>