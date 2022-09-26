<script>
export default {
    name: 'FeaturesButton',
    data(){
            return {
                select: false,
                highlight: {

        background: "white",
    },

           

}


            },

             props: {
                title: String,
            }, 
        

    methods: {
        



 selected() {
            

     this.select = !this.select


  }
    }

}
</script>

<template>
    <div>
        <button @click="selected"  id="btn" class="btn text-lg mx-2 border  px-4 py-1 rounded-xl  hover:shadow hover:backdrop-blur hover:rounded-xl border-none ">{{title}}</button>
    </div>
</template>


<style>
.btn:hover {
    background-color:rgba(214, 210, 210, 0.115) ;
}



</style>