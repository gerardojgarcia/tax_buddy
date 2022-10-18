<script>
export default {
  name: "FAQ",

  data(){

    return {
      faq: []
    }


  },

  created(){
    this.faq = [
        {
      id: 1,
      question: "Does TaxBuddy handle sales tax?",
      answer: "Well no, but if you move your company offshore you can probably ignore it."
    },

      {
        id: 2,
        question: "Can i pay for my subscription via purchase order?",
        answer: "Absolutely, we are happy to take your money in all forms."
      },
      {
        id: 3,
        question: "How do I apply for a job at TaxBuddy",
        answer: "We only hire our customers, so subscribe for a minim of 6 months and then let's talk."
      },
      {
        id: 4,
        question: "What was that testimonial about tax fraud all about",
        answer: "TaxBuddy is just a software application, ultimately your books are your responsibility"
      },
      {
        id: 5,
        question: "TaxBuddy sounds excellent, I fell compelled to purchase",
        answer: "This is the power of superior visual design. You just can't resisst it, no matter how poorly it actually functions."
      },
      {
        id: 6,
        question: "I found other companies called TaxBuddy, are you sure you can use this name?",
        answer: "Honestly, not sure at all. We haven't actually icorporated or antying, we just hought it sounded cool and made this website. "
      },


    ]
  },


}
</script>


<template>

  <div class="w-full m-auto text-left px-4 my-16 md:px-60 md:pt-16">
    <strong class="text-4xl md:text-5xl font-normal">Frequently Asked Questions
    </strong>

    <p class="text-xl text-gray-600 md:text-lg my-8 font-light md:w-2/5">if you can't find what you're looking for, email our support team and if you're lucky someone wil get back to you</p>


  </div>

  <div class="flex flex-wrap md:px-60 md:flex-row md:w-full self-center m-auto md:pb-32">

    <!--Container for faq cards-->
    <div class="faq-cards md:w-2/6 " v-for="card in faq" :key="card.id">

  <!--Individual FAQ Card-->
        <div class="faq-card w-full  text-left px-4 md:px-3 md:mb-8 mt-6">
          <strong class="text-xl font-normal md:text-2xl">{{card.question}}</strong>
          <p class="py-4 text-md md md:w-3/4 text-gray-600">{{card.answer}}</p>

        </div>


    </div>
  </div>

</template>





<style scoped>

</style>