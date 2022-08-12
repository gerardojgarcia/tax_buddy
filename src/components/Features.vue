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

        payroll.classList.toggle('display')
        payrollBtn.classList.toggle('selected')

        claim.classList.add('display')
        claimBtn.classList.remove('selected')

         report.classList.add('display')
        reportBtn.classList.remove('selected')

        


    },
    claim(){

        const payroll = document.querySelector('#payroll')
        const payrollBtn = document.querySelector('#payroll-btn')

        const claim = document.querySelector('#claim')
        const claimBtn = document.querySelector('#claim-btn')

        const report = document.querySelector('#report')
        const reportBtn = document.querySelector('#report-btn')

        payroll.classList.add('display')
        payrollBtn.classList.remove('selected')

        claim.classList.toggle('display')
        claimBtn.classList.toggle('selected')

    report.classList.add('display')
        reportBtn.classList.remove('selected')


    },

    report(){
        const payroll = document.querySelector('#payroll')
        const payrollBtn = document.querySelector('#payroll-btn')
        const claim = document.querySelector('#claim')
        const claimBtn = document.querySelector('#claim-btn')
        const report = document.querySelector('#report')
        const reportBtn = document.querySelector('#report-btn')


        report.classList.toggle('display')
        reportBtn.classList.toggle('selected')

        claim.classList.add('display')
        claimBtn.classList.remove('selected')
          payroll.classList.add('display')
        payrollBtn.classList.remove('selected')

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

        <div class="feature-description text-gray-300 px-4">
            <p id="payroll" class=" ">Keep track of everyone's salaries and whether or not they've been paid. Direct deposit not supported.</p>
            <p id="claim" class="display">All of your receipts organized into one place, as long as you don't mind typing in the data by hand.</p>
            
            <p id="report" class="display">Easily export your data into an Excel spreadsheet where you can do whatever the hell you want with it.</p>
        </div>

        <div class="features-img">
        
            <img src="/" alt="">
            <img src="" alt="">
            <img src="" alt="">
        
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
    color: black;
}


.display {
    display: none;
}
</style>