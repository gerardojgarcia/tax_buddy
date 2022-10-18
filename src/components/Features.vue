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

    },

    payrollLarge(){
        const payrollLg = document.getElementById('payroll-el')
        const payrollImgLg = document.getElementById('report-img-lg')
        const claimLg = document.getElementById('claim-el')
            const claimImgLg = document.getElementById('claim-img-lg')
            const reportLg = document.getElementById('report-el')
        const reportImgLg = document.getElementById('expense-img-lg')

        console.log( 'i was clicked')

        payrollLg.classList.toggle("active")
        payrollImgLg.classList.toggle('display')

        claimLg.classList.remove('active')
            claimImgLg.classList.add('display')

            reportLg.classList.remove('active')
        reportImgLg.classList.add('display')




    },

    claimLarge(){

            const claimLg = document.getElementById('claim-el')
            const claimImgLg = document.getElementById('claim-img-lg')
            const payrollLg = document.getElementById('payroll-el')
        const payrollImgLg = document.getElementById('report-img-lg')
        const reportLg = document.getElementById('report-el')
        const reportImgLg = document.getElementById('expense-img-lg')
            

            claimLg.classList.toggle('active')
            claimImgLg.classList.toggle('display')

            payrollLg.classList.remove("active")
        payrollImgLg.classList.add('display')


        reportLg.classList.remove('active')
        reportImgLg.classList.add('display')


        
    },

    reportLarge() {
        const claimLg = document.getElementById('claim-el')
            const claimImgLg = document.getElementById('claim-img-lg')
            const payrollLg = document.getElementById('payroll-el')
        const payrollImgLg = document.getElementById('report-img-lg')
        const reportLg = document.getElementById('report-el')
        const reportImgLg = document.getElementById('expense-img-lg')



        reportLg.classList.toggle('active')
        reportImgLg.classList.toggle('display')



        claimLg.classList.remove('active')
            claimImgLg.classList.add('display')

            payrollLg.classList.remove("active")
        payrollImgLg.classList.add('display')



    }


}

}

             


        

</script>

<template>
    <div class="features-container flex flex-col justify-center items-center pt-16 pb-32 ">

    <div class="features-header text-left px-4 lg:mb-8 lg:text-center">
    
        <div class=" mb-8 mt-6 lg:mb-8 lg:mt-16">
        <strong class="text-4xl font-normal text-white lg:text-5xl ">Everything you need to run your books.</strong>
        </div>
    
    <p class="text-gray-200 text-lg lg:text-lg">Well, everything you need if you aren't that picky about minor details like tax compliance. </p>


    
    </div>

    <div class="features-box w-auto mx-4 mt-16 pb-8 rounded-lg  backdrop-blur-lg md:backdrop-blur-none bg-transparent lg:shadow-none shadow-lg">
        <div class="features-tabs flex flex-row pt-8 pb-4 items-center justify-center lg:hidden">


            


            <FeaturesButton id="payroll-btn" title="Payroll" @click='payroll' class="selected text-gray-200" />

            
            <FeaturesButton id="claim-btn" title="Claim expenses" @click="claim" class="text-gray-200" />

            <FeaturesButton id="report-btn" title="Reporting" @click="report" class="text-gray-200"/>

        
        
        </div>

        <div class="feature-description text-left flex flex-col items-center my-4 pb-6 text-gray-300 px-4 lg:hidden">
            <p id="payroll" class=" w-1/2 ">Keep track of everyone's salaries and whether or not they've been paid. Direct deposit not supported.</p>
            <p id="claim" class="display w-1/2">All of your receipts organized into one place, as long as you don't mind typing in the data by hand.</p>
            
            <p id="report" class="display w-1/2">Easily export your data into an Excel spreadsheet where you can do whatever the hell you want with it.</p>
        </div>

        <div class="features-imgs lg:hidden">
        
            <img src="/claims.png" id="claim-img" alt="Image of the claims dashboard" class="feature-img translate-x-52  shadow-lg display">
            <img src="/reports.png" id="report-img" alt="Image of the reports dashboard" class="feature-img translate-x-52  shadow-lg">
            <img src="/expenses.png" id="expense-img" alt="Image of the expenses dashboard" class="feature-img display translate-x-52  shadow-lg">
        
        </div>


        <!-- features container for large screens-->
        <div class="lg-features-container hidden lg:flex lg:flex-row items-center w-5/6 m-auto">   

        <div class="flex flex-col text-left text-white w-2/5">
            <div @click="payrollLarge" id="payroll-el" class=" active w-full mb-8 hover:rounded-xl hover:shadow-lg p-4  cursor-pointer" >
            
                <div >
                <strong class="text-xl">Payroll</strong>
                </div>
                <p id="payroll" >Keep track of everyone's salaries and whether or not they've been paid. Direct deposit not supported.</p>
            
            
            </div>
            <div @click="claimLarge" id="claim-el" class="w-full mb-8 hover:rounded-xl hover:shadow-lg p-4 cursor-pointer">
            
            <strong class="text-xl">Claim</strong>
            <p >Keep track of everyone's salaries and whether or not they've been paid. Direct deposit not supported.</p>
                
                
                </div>
                <div @click="reportLarge" id="report-el" class="w-full mb-8 hover:rounded-xl hover:shadow-lg p-4 cursor-pointer">
            
            <strong class="text-xl">Report</strong>
            <p  >Keep track of everyone's salaries and whether or not they've been paid. Direct deposit not supported.</p>
                
                
                </div>
        </div>
        
        
    <div class="lg-img-container w-3/5">
        
        
        
        <img src="/claims.png" id="claim-img-lg" alt="Image of the claims dashboard" class="feature-img translate-x-8  shadow-lg display">
        <img src="/reports.png" id="report-img-lg" alt="Image of the reports dashboard" class="feature-img translate-x-8  shadow-lg">
        <img src="/expenses.png" id="expense-img-lg" alt="Image of the expenses dashboard" class="feature-img display translate-x-8  shadow-lg">
    
    
    
    
    </div>


</div>
        
        
        </div>


        
        
    </div>
</template>


<style scoped>


    .features-container {
        background: linear-gradient(rgb(42, 42, 239), rgb(113, 149, 255));
        overflow: hidden;
    }

    .features-box {
        background-color: rgba(214, 210, 210, 0.115);
    }

    @media (min-width:800px){
        .features-box {
            background: none;
             
        }
    }





.selected {
    background-color: white;
    border-radius: 50rem;
    color: #2563ea;
}


.active {
    background-color: rgba(255, 255, 255, 0.144);
    border-radius: .5rem;
    box-shadow: 0 10px 15px -3px rgb(0 0 0 / 0.1), 0 4px 6px -4px rgb(0 0 0 / 0.1);
    border:none;
    color: whitesmoke;
}

.display {
    display: none;
}

.feature-img {
    height: 500px;
    min-width: 800px;

    z-index: 3;

}


@media (min-width: 800px){
    .feature-img {
        height: 800px;
        min-width: 1000px;


    }
}
</style>