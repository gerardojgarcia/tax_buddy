<script>

    import Nav from './Nav.vue';
    import HeaderButton from './HeaderButton.vue';


export default {
    name: 'Header',

    components: {
            Nav,
            HeaderButton,
}

}


</script>
<template>

<header class="w-full flex flex-row items-center justify-between py-8 px-4">
<div>

    <p class="text-black text-2xl font-bold"><span class="text-blue-700">Tax</span>Buddy</p>

</div>
   


    <div>
    
    <Nav class="w-1/3 hidden lg:flex lg:flex-row"/>
    
    
    </div>


    <div class="ml-20">
        <a href="#" class="hidden lg:inline">Sign In</a>

       <div>
       
        <HeaderButton />
       </div>
    
    </div>

    <div class="hamburger-btn w-8 inline place-center cursor-pointer">
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