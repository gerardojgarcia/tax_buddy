<script>

    import Nav from './Nav.vue'


export default {
    name: 'Header',

    components: {
        Nav,
    }

}


</script>
<template>

<header class="w-full flex flex-row items-center justify-between py-6 px-4">
<img src="#" alt="TaxBuddy" class="logo">
   


    <div>
    
    <Nav class="w-1/3 hidden lg:flex lg:flex-row"/>
    
    
    </div>


    <div class="ml-36">
        <a href="#" class="hidden lg:inline">Sign In</a>

        <button class="header-btn bg-blue-600 py-1 px-2  rounded-full hover:bg-blue-700">Get Started <span class="hidden lg:inline">Today</span></button>
    
    </div>

    <div class="hamburger-btn w-8 inline place-center ">
        <div class="burger-top w-5 my-1  bg-black "></div>
        <div class="burger-middle w-5 my-1 bg-black "></div>
        <div class="burger-bottom w-5 my-1 bg-black "></div>

    
    
    
    </div>


</header>



</template>


<style>

    .burger-top, .burger-middle, .burger-bottom {
        height: 2px;

    }



</style>