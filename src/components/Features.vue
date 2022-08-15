<script>
import FeaturesButton from './FeaturesButton.vue'
export default {
    name: 'Features',

components: {
    FeaturesButton,
},

props: {
    title: String,
},
methods: {
    payroll(){
        const payroll = document.querySelector('#payroll')
        const payrollBtn = document.querySelector('#payroll-btn')
        const claim = document.querySelector('#claim')
        const claimBtn = document.querySelector('#claim-btn')

        const report = document.querySelector('#report')
        const reportBtn = document.querySelector('#report-btn')

        const claimImg = document.getElementById('claim-img')
         const reportImg = document.getElementById('report-img')
          const expenseImg = document.getElementById('expense-img')

        payroll.classList.toggle('display')
        payrollBtn.classList.toggle('selected')

        claim.classList.add('display')
        claimBtn.classList.remove('selected')

         report.classList.add('display')
        reportBtn.classList.remove('selected')

        claimImg.classList.add('display')
        expenseImg.classList.add('display')

        reportImg.classList.remove('display')

        


    },
    claim(){

        const payroll = document.querySelector('#payroll')
        const payrollBtn = document.querySelector('#payroll-btn')

        const claim = document.querySelector('#claim')
        const claimBtn = document.querySelector('#claim-btn')

        const report = document.querySelector('#report')
        const reportBtn = document.querySelector('#report-btn')

        const claimImg = document.getElementById('claim-img')
         const reportImg = document.getElementById('report-img')
          const expenseImg = document.getElementById('expense-img')

        payroll.classList.add('display')
        payrollBtn.classList.remove('selected')

        claim.classList.toggle('display')
        claimBtn.classList.toggle('selected')

        report.classList.add('display')
        reportBtn.classList.remove('selected')

        reportImg.classList.add('display')
        expenseImg.classList.add('display')
        claimImg.classList.remove('display')




    },

    report(){
        const payroll = document.querySelector('#payroll')
        const payrollBtn = document.querySelector('#payroll-btn')
        const claim = document.querySelector('#claim')
        const claimBtn = document.querySelector('#claim-btn')
        const report = document.querySelector('#report')
        const reportBtn = document.querySelector('#report-btn')

         const claimImg = document.getElementById('claim-img')
         const reportImg = document.getElementById('report-img')
          const expenseImg = document.getElementById('expense-img')


        report.classList.toggle('display')
        reportBtn.classList.toggle('selected')

        claim.classList.add('display')
        claimBtn.classList.remove('selected')
          payroll.classList.add('display')
        payrollBtn.classList.remove('selected')

          claimImg.classList.add('display')
        expenseImg.classList.remove('display')
        reportImg.classList.add('display')

    }
}

}

             


        

</script>

<template>
    <div class="features-container flex flex-col justify-center items-center pt-16 pb-32">

    <div class="features-header text-left px-4">
    
        <strong class="text-2xl text-white">Everything you need to run your books.</strong>
    
    <p class="text-white">Well, everything you need if you aren't that picky about minor details like tax compliance. </p>


    
    </div>

    <div class="features-box w-auto mx-4 mt-16 pb-8 rounded-lg  backdrop-blur-lg shadow-lg">
        <div class="features-tabs flex flex-row py-4 items-center justify-center">


            


            <FeaturesButton id="payroll-btn" title="Payroll" @click='payroll' class="selected"/>

            
            <FeaturesButton id="claim-btn" title="Claim Expense" @click="claim" />

            <FeaturesButton id="report-btn" title="Reporting" @click="report"/>

        
        
        </div>

        <div class="feature-description text-left flex flex-col items-center my-4 text-gray-300 px-4">
            <p id="payroll" class=" w-1/2 ">Keep track of everyone's salaries and whether or not they've been paid. Direct deposit not supported.</p>
            <p id="claim" class="display w-1/2">All of your receipts organized into one place, as long as you don't mind typing in the data by hand.</p>
            
            <p id="report" class="display w-1/2">Easily export your data into an Excel spreadsheet where you can do whatever the hell you want with it.</p>
        </div>

        <div class="features-imgs">
        
            <img src="/claims.png" id="claim-img" alt="Image of the claims dashboard" class="feature-img translate-x-52  shadow-lg display">
            <img src="/reports.png" id="report-img" alt="Image of the reports dashboard" class="feature-img translate-x-52  shadow-lg">
            <img src="/expenses.png" id="expense-img" alt="Image of the expenses dashboard" class="feature-img display translate-x-52  shadow-lg">
        
        </div>
    </div>
        
    </div>
</template>


<style scoped>


    .features-container {
        background: linear-gradient(rgb(81, 81, 253), rgb(113, 149, 255));
    }

    .features-box {
        background-color: rgba(214, 210, 210, 0.115);
    }





.selected {
    background-color: white;
    border-radius: 50rem;
    color: rgb(48, 48, 224);
}


.display {
    display: none;
}

.feature-img {
    height: 500px;
    min-width: 800px;

    z-index: 3;

}
</style>