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
<div class="flex lg:items-center lg:ml-40">

    <p class="text-black text-2xl font-bold"><span class="text-blue-700">Tax</span>Buddy</p>
    <Nav class="w-1/3 hidden lg:flex lg:flex-row lg:ml-8"/>

</div>
   


    


    <div class="ml-20 lg:flex lg:items-center lg:mr-40">
        <a href="#" class="hidden lg:inline lg:mr-16">Sign In</a>

       <div>
       
        <HeaderButton />
       </div>
    
    </div>

    <div class="hamburger-btn w-8 inline place-center cursor-pointer lg:hidden">
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