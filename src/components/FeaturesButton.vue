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
        <button @click="selected"  id="btn" class="btn mx-2 border text-gray-300 px-4 py-1 rounded-xl  hover:shadow hover:backdrop-blur hover:rounded-xl border-none focus:text-blue-300 focus:shadow-lg">{{title}}</button>
    </div>
</template>


<style>
.btn:hover {
    background-color:rgba(214, 210, 210, 0.115) ;
}

.selected {
    background-color: white;
    border-radius: 50rem;
    color: black;
}

</style>