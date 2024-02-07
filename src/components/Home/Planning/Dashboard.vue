<script setup>
    import Header from '../Header.vue';
    import Graph1 from './graph/Dashboard/graph1.vue';
    import Graph2 from './graph/Dashboard/graph2.vue';
    import Graph3 from './graph/Dashboard/graph3.vue';
    import Enrollment from './graph/Dashboard/enrollment.vue';
    import Graduates from './graph/Dashboard/graduates.vue';
    import Scholarship from './graph/Dashboard/scholarship.vue'
    import PassingRate from './graph/Dashboard/passing_rate.vue'
    import Research from './graph/Dashboard/research.vue';
    import Research2 from './graph/Dashboard/research2.vue';
    import Footer from '../footer.vue'
</script>

<template>
    <Header/>
    
    <div
        id="PL_db_main"
    >
    <section 
        id ="PL_db_sec1"
        class="w-100"
        style="padding: 6rem 3rem 5rem 6rem;background-color: white;"
    >

        <h1 
            class="d-flex flex-column w-100 text-red-darken-4 text-h3 font-weight-black"
        >
            University Management 
            <span class="text-red-darken-1 mt-2">Information <span class="text-red-darken-4">System</span> </span> 
        </h1>

        <div class="w-100 d-flex">
            <p 
                class="d-flex mt-4 text-grey-darken-3"
                style="width: 40%;border:"
            >
                Central System for Managing and Processing data 
                <br> of Batangas State University
            </p>

            <span 
                class="d-flex"
                style="width: 60%;border: "
                id = "PL_db_subnav"
            >
                <ul>
                    <li>Overview</li>
                    <li> QR Stars</li>
                    <li>THE</li>
                    <li>Scopus</li>
                    <li>Altmetric</li>
                </ul>
            </span>
        </div>

        <div class="w-100 d-flex flex-wrap">
            
            <h1 
                class="w-100 text-red-darken-4"
                style="margin-top: 5rem;"
            >
                Faculty Profile
            </h1>

            <span 
                class="w-50 pt-8"
                style=" display: flex;justify-content: center;"
            >
                <Graph1/>
            </span>

            <span 
                class="w-50 pt-8"
                style=" display: flex;justify-content: center;"
            >
                <Graph2/>
            </span>
        </div>
    </section>

    <section
        class="w-100"
        id="PL_db_sec2"
        style="display: flex;justify-content: center; align-items: flex-end; background-color: white; "
    >
        <Graph3/>
    </section>


    <section
        class="w-100 d-flex flex-column align-center"
        id = "PL_db_sec3"
        style="padding: 4rem 3rem 5rem 6rem;"
        
    >
        <h1 
            class="w-100 text-red-darken-4"
            
        >
            College Statistics
        </h1>

        <div class="w-100 d-flex flex-wrap justify-center ">
            <v-card 
                class=" my-8 d-flex justify-end"  
                style="width: 45%;margin-right: 2em;"
            >
                <Enrollment/>
            </v-card >
            <v-card 
                class="my-8  d-flex justify-start" 
                style=" width: 45%;"
            >
                <Graduates/>
            </v-card>
            <v-card 
                class="py-8  d-flex justify-end" 
                style=" width: 45%;margin-right: 2em"
            > 
                <Scholarship/>
            </v-card>
            <v-card
                class="py-8  d-flex justify-start" 
                style=" width: 45%;"
            >

            </v-card>

        </div>

        <v-card class=" d-flex mt-8 justify-center py-16" style="width: 92%;">
                <PassingRate/>
        </v-card>

    </section>

    <section
        class="w-100 d-flex flex-column align-center"
        id = "PL_db_sec4"
        style="padding: 4rem 3rem 5rem 6rem;background-color: white;"
    >
        <h1 
            class="w-100 text-red-darken-4"  
        >
            Extension Services
        </h1>

        <div class="d-flex mt-8  flex-wrap" style=" width: 90%;">
            <v-card  class ="PL_db_extServ" elevation="2">
                <img src="../../../assets/img/extension/7.png" alt="">
                <h3>2</h3>
                <p>Fund Raising for Community Development</p>
            </v-card>
            <v-card  class ="PL_db_extServ" elevation="2">
                <img src="../../../assets/img/extension/2.png" alt="" style="width: 13%;">
                <h3>9</h3>
                <p>Clean and Green Community / Coatal Cleanup</p>
            </v-card>
            <v-card  class ="PL_db_extServ" elevation="2">
                <img src="../../../assets/img/extension/4.png" alt="" style="width: 11%;">
                <h3>22</h3>
                <p>Tree Planting</p>
            </v-card>
            <v-card  class ="PL_db_extServ" elevation="2">
                <img src="../../../assets/img/extension/6.png" alt="" style="width: 11%;">
                <h3>15  </h3>
                <p>Food and Nutrition / Health and Sanitation / Material and Child Care</p>
            </v-card>            
        </div>

        <div class="d-flex mt-8  flex-wrap" style=" width: 90%;">
            <v-card  class ="PL_db_extServ" elevation="2">
                <img src="../../../assets/img/extension/1.png" alt="" style="width: 11%;">
                <h3>2</h3>
                <p>Youth sports development environment camps</p>
            </v-card>
            <v-card  class ="PL_db_extServ" elevation="2">
                <img src="../../../assets/img/extension/3.png" alt="" style="width: 11%;">
                <h3>9</h3>
                <p>Gift Giving Activity</p>
            </v-card>
            <v-card  class ="PL_db_extServ" elevation="2">
                <img src="../../../assets/img/extension/5.png" alt="" style="width: 10%;">
                <h3>22</h3>
                <p>Blood Donation</p>
            </v-card>           
        </div>

        <h1 
            class="w-100 text-red-darken-4 mt-16"  
        >
            Accreditation status of Academic Programs
        </h1>

        
        <div
            class="d-flex justify-space-between mt-16"
            style="width: 60%;"
        >

            <v-card class="PL_db_research">
               
                <h4>6</h4>
                <p>ABET Accredited</p>
            </v-card>
            <v-card class="PL_db_research">
                <h4>5</h4>
                <p>Qualified for Level 4</p>
            </v-card>
            <v-card class="PL_db_research">
                <h4>4</h4>
                <p>Level IV Phase I</p>
            </v-card>
            <v-card class="PL_db_research">
                <h4>4</h4>
                <p>Qualified for Level III</p>
            </v-card>
        </div>

        <div
            class="d-flex justify-space-between mt-8"
            style="width: 60%;"
        >

            <v-card class="PL_db_research">
                <h4>4</h4>
                <p>Level III Re-accredited</p>
            </v-card>
            <v-card class="PL_db_research">
                <h4>31</h4>
                <p>Level II Re-accredited</p>
            </v-card>
            <v-card class="PL_db_research">
                <h4>50</h4>
                <p>Level I Accredited</p>
            </v-card>
            <v-card class="PL_db_research">
                <h4>12</h4>
                <p>Candidates</p>
            </v-card>
        </div>
    </section>

    <section 
            class="w-100 d-flex flex-column align-center"
            id = "PL_db_sec5"
            style="padding: 4rem 3rem 5rem 6rem;"
    >
            <h1 
                class="w-100 text-red-darken-4"  
            >
                Extension Services
            </h1>
            
            <div class="w-75 d-flex mt-8" >
                <span class="w-50 d-flex justify-center">
                    <Research/>
                </span>
                <span class="w-50 d-flex justify-center">
                    <Research2/>
                </span>
            </div>

            <div style="width: 60%;display: flex;gap: 4em;margin: 6rem 0 0 0;">
                <v-card class="PL_db_research text-center">
                    <h4>90</h4>
                    <p>Full time researchers with research project</p>
                </v-card>
                <v-card class="PL_db_research text-center ">
                    <h4>7</h4>
                    <p>On-going externally-funded research projects</p>
                </v-card>
                <v-card class="PL_db_research text-center">
                    <h4>90</h4>
                    <p>Completed externally-funded research projects</p>
                </v-card>
                <v-card class="PL_db_research text-center">
                    <h4>90</h4>
                    <p>Intellectual property assets</p>
                </v-card>
  
            </div>
    </section>

        <Footer/>

</div>
</template>

<style scoped>
    :root{
        --red-darken-4:#B71C1C;   
    }
    #PL_db_main{
        width: 100%;

    }

    #PL_db_subnav > ul{
        width: 100%;
        list-style-type: none;
        display: flex;
        align-items: center;
        justify-content: flex-end;
        gap: 1em;
    }

   .PL_db_subnav > ul > li{
        text-align: center;
        padding: .5em 0em;
        width:15%;
    }

    .PL_db_subnav > ul > li:hover{
        background-color: #B71C1C;
        color: white;
    }
    
    .PL_db_extServ{
        width: 22%;
        display: flex;
        align-items: center;
        padding: .4rem 1.2rem;
        margin: 0 2rem 0 0;

    }
    .PL_db_extServ > img{
        width: 20%;
        height: auto;
    }
    .PL_db_extServ > h3{
        color: #E53935;
        padding: 0 20px 0 10px;
        font-size: 30px;
    }
    .PL_db_extServ > p{
        width: 60%;
        font-size: 15px;
    }

    .PL_db_research{
        display: flex;
        flex-direction: column;
        align-items: center;
        padding: 1em 2em;
        position: relative;
        width: 23%;
    }
    .PL_db_research:hover {
        background-color: #B71C1C;
        color: white;
     
        & > h4{
            color: white;
        }
    }


    .PL_db_research > h4{
        color: #E53935;
        font-size: 35px;
    }

    .PL_db_research > p{
        max-width: 100%;
    }

</style>