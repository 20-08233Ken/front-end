<script setup>

    import Graph1 from './graph/graph1.vue';
    import Graph2 from './graph/graph2.vue';
    import Graph3 from './graph/graph3.vue';

</script>

<template>
    <div id ="w-100 planning_landing d-flex flex-column">
        

        <!-- section-1 -->
        <section id="PL_section_1" class="w-100 d-flex flex-column" style="display: flex; flex-direction: column;">
            <div class="d-flex">
                  <!-- Left Section -->
                <span class="d-flex w-50 flex-column" style="margin:6rem 0 0 6rem;"> 

                    <h1 class="d-flex flex-column w-100 text-red-darken-4 text-h3 font-weight-black">
                        University Management 
                        <span class="text-red-darken-1 mt-2">Information <span class="text-red-darken-4">System</span> </span> 
                    </h1>

                    <p class="w-50 mt-4 text-grey-darken-3">
                        Central System for Managing and Processing data <br> of Batangas State University
                    </p>

                    <p class="w-75 mt-8 text-grey-darken-3 text-subtitle-1">
                        Lorem ipsum dolor sit amet consectetur adipisicing elit. Illo quidem placeat veritatis
                        accusantium laborum dignissimos animi? Maiores labore ducimus distinctio vero a fugiat
                        autem dolore optio sapiente magnam! Veniam, at.
                        accusantium laborum dignissimos animi? Maiores labore ducimus distinctio vero a fugiat
                        autem dolore optio sapiente magnam! Veniam, at.
                    </p>
                </span>

                 <!-- Right Section -->
                <span class="d-flex flex-column w-50 align-center justify-center"  id ="PL_landing_sec2_img">

                    <img src="../../../assets/img/merge/img1.png" alt="">                

                </span>
            </div>

            <!-- Search Section -->
            <div class="w-100 d-flex justify-center" style=" margin: 4rem 0 0 0; ">

                <span class="w-50">
                    <h1 class="mb-4 text-red-darken-4" style="font-family: Inter-Bold;">Search for an Office</h1>

                    <span id ="PL_landing_search" >
                        <input type="text" name="" id="PL_landing_search_input" placeholder="Seacrch">
                        <v-btn elevation="0" style="width: 2%;">
                            <v-icon icon class="px-10 py-5 mx-auto">
                                mdi-magnify
                            </v-icon>
                        </v-btn>
                    </span>
                </span>
            </div>

             <!-- Offices Section -->
            <div class="w-100 d-flex flex-column align-center">

                <span class=" d-flex flex-column"  style="width: 90%;margin-top: 2em;">
                    <h1 class="text-white">Head Offices</h1>
                    <p class="text-white text-subtitle-2" style="font-family: Inter-Regular;">Find your Office under these head offices</p>
                </span>

                <span class="d-flex mt-8 justify-space-evenly" style="width: 90%;">
                        <v-card
                           
                            class="PL_landing_office_card"
                        >
                            <h1>OUP</h1>
                            <p >Office of the University President</p>
                        </v-card>

                        <v-card
                  
                            class="PL_landing_office_card"
                        >
                            <h1>OVP <span>AA</span></h1>
                            <p>Office of the Vice President for Academic Affairs</p>
                        </v-card>

                        <v-card
                       
                            class="PL_landing_office_card"
                        >
                            <h1>OVP <span>RDES</span></h1>
                            <p>Office of the Vice President for  Research, Development, and Extension Services</p>                          
                        </v-card>

                        <v-card
                         
                            class="PL_landing_office_card"
                        >
                            <h1>OVP <span>AF</span></h1>
                            <p>Office of the Vice President for  Administration and Finance</p>           
                        </v-card>
                        <v-card
                          
                            class="PL_landing_office_card"
                        >
                            <h1 style="font-family: 'Roboto';">OVP <span>DEA</span></h1>
                            <p>Office of the Vice President for Development and External  Affairs</p>                          
                        </v-card>
                </span>


                <span class="mt-8 pb-8">
                    <v-btn class="text-white rounded-lg" style="background-color: #880f0f;">See more Offices</v-btn>
                </span>



            </div>
        </section>

        <!-- section-2 -->
        <section id="PL_section_2" class="d-flex flex-column" >

            <span class="d-flex w-100">
                <div class="w-50" style="width: 40%; padding: 9rem 0 0 6rem;">
                    
                    <h1 class="d-flex flex-column text-h3 text-red-darken-3" style="font-family: Inter-Bold;">University Data 
                        <span class="text-red-darken-1" style="font-family: Inter-Bold;" >Dashboard</span>
                    </h1>

                    <p class="mt-8" style="width: 60%;">Monitor overall data gathered within the university. Process those data and visualize those data into more understandable presentation.</p>
                    <p class="mt-8" style="width: 60%;">Help visualize the trajectory of the university through visualizing data from criterion of different university rankings.</p>
                </div>
                <div class="d-flex mt-16"  style="width: 50%;">
                    <Graph1/>
                    <Graph2/>
                </div>
            </span>



                <div class="w-100" style="height: 75vh;" >
                    <Graph3/>
                </div>
            
        </section>

        <!-- section-3 -->
        <section id ="PL_section_4" class="w-100 d-flex flex-wrap"> 
                
            <span class="w-50" > 
                <h1 class="d-flex w-100 text-red-darken-4 text-h3 font-weight-black" style="font-family: Inter-Bold;">University
                     <span class="text-red-darken-1 ml-4" style="font-family: Inter-Bold;">Facts</span>
                </h1>
                <h1 class="d-flex w-100 text-red-darken-4 text-h3 font-weight-black mt-2" style="font-family: Inter-Bold;">
                     and 
                     <span  class="text-red-darken-1 ml-4" style="font-family: Inter-Bold;">Figures</span>
                </h1>
              

                <p class="mt-8 w-75">View the university’s facts and information coming from data gathered within the whole school year.</p>
                <p class="mt-8 w-75">Showcase the capabilities of the university through organized report and data visualization</p>

                <v-btn color ="red-darken-4" class="d-flex justify-flex-start text-subtitle-2 py-6 w-75" 
                            style="margin-top: 10rem;
                                    max-width: 100%;
                                    overflow: hidden;
                                text-overflow: ellipsis;">
                    <img src="../../../assets/img/icons8-pdf-50.png" alt="" style="width: 9%;margin-right: 1em;">
                    <p class="d-flex w-100 text-center;">
                        Download BatStateU Facts and Figures
                    </p>
                </v-btn>
            
                <p class="w-75 text-center mt-4"> <u> View University Facts and Figures Table of Contents</u></p>
            </span>
                
            <span class="w-50 d-flex align-center justify-center flex-wrap">
                <img src="../../../assets/img/dash.png" alt="" style="max-width: 65%;width: 100%;">

            </span>
        </section>

        <div class="w-100 d-flex" style="background-color: #D9D9D9;">
        <h1 
            class="w-50 text-white" 
            style="padding:  1rem 0 0 6rem; background-color: #D00412; clip-path: polygon(0 0, 95% 0, 100% 100%, 0% 100%);">
            University Dataset
        </h1>
        </div>

        <!-- setion-4 -->
        <section 
            class="w-100 d-flex align-center pb-16"
            style="background-color: #D00412"
        >
                <div 
                    class="d-flex w-50 " 
                    style="margin:3rem 0 0 6rem;;
                ">
                  <!-- Card 1 -->  
                    <v-card class="w-50 w-50" style="border-radius: 10px; border:1px solid white;">
                        <h3 
                            class="w-100 d-flex align-center justify-space-evenly text-white py-4"
                            style="background-color: #94080D;">
                            <img 
                                src="../../../assets/img/qs-stars.png  " 
                                style="width: 20%;height: auto;"
                                alt="" srcset="">
                            <p>QR Stars Data Criteria</p>
                        </h3>

                        <!-- List 1 --> 
                        <h4 
                            class="px-4 py-4"
                        >
                            Culture and Arts
                        </h4>
                        
                        <ul
                            class="px-16"
                        >
                            <li>Lorem ipsum dolor sit amet, consectetur adipiscing elit</li>
                            <li>Maecenas vehicula purus vitae sapien malesuada, eget pretium justo lacinia.</li>
                            <li>Aliquam ac ipsum auctor, dictum ex vitae, placerat nisi.</li>
                            <li>Suspendisse dictum leo eu nibh pretium, et finibus turpis porta.</li>
                        </ul>

                        <!-- List 2 --> 
                                                <h4 
                            class="px-4 py-4"
                        >
                            Sports
                        </h4>
                        
                        <ul
                            class="px-16"
                        >
                            <li>Lorem ipsum dolor sit amet, consectetur adipiscing elit</li>
                            <li>Maecenas vehicula purus vitae sapien malesuada, eget pretium justo lacinia.</li>
                            <li>Aliquam ac ipsum auctor, dictum ex vitae, placerat nisi.</li>
                            <li>Suspendisse dictum leo eu nibh pretium, et finibus turpis porta.</li>
                        </ul>


                        <!-- List 3 --> 
                                                <h4 
                            class="px-4 py-4"
                        >
                            Teaching
                        </h4>
                        
                        <ul
                            class="px-16"
                        >
                            <li>Lorem ipsum dolor sit amet, consectetur adipiscing elit</li>
                            <li>Maecenas vehicula purus vitae sapien malesuada, eget pretium justo lacinia.</li>
                            <li>Aliquam ac ipsum auctor, dictum ex vitae, placerat nisi.</li>
                            <li>Suspendisse dictum leo eu nibh pretium, et finibus turpis porta.</li>
                        </ul>

                        <v-btn class="w-100 mt-8 d-flex text-white" style="background-color:#880f0f;">
                            <p class="text-subtitle-2 mr-4"> View More</p>
                            <v-icon icon>mdi-arrow-right-circle</v-icon>
                        </v-btn>
                    </v-card>


                    <!-- Card 2 -->  
                    <v-card class="w-50 w-50 mx-8" style="border-radius: 10px; border:1px solid white;">
                        <h3 
                            class="w-100 d-flex align-center justify-space-evenly text-white py-4"
                            style="background-color: #94080D;">
                            <img 
                                src="../../../assets/img/qs-stars.png  " 
                                style="width: 20%;height: auto;"
                                alt="" srcset="">
                            <p>QR Stars Data Criteria</p>
                        </h3>

                        <!-- List 1 --> 
                        <h4 
                            class="px-4 py-4"
                        >
                            Culture and Arts
                        </h4>
                        
                        <ul
                            class="px-16"
                        >
                            <li>Lorem ipsum dolor sit amet, consectetur adipiscing elit</li>
                            <li>Maecenas vehicula purus vitae sapien malesuada, eget pretium justo lacinia.</li>
                            <li>Aliquam ac ipsum auctor, dictum ex vitae, placerat nisi.</li>
                            <li>Suspendisse dictum leo eu nibh pretium, et finibus turpis porta.</li>
                        </ul>

                        <!-- List 2 --> 
                                                <h4 
                            class="px-4 py-4"
                        >
                            Sports
                        </h4>
                        
                        <ul
                            class="px-16"
                        >
                            <li>Lorem ipsum dolor sit amet, consectetur adipiscing elit</li>
                            <li>Maecenas vehicula purus vitae sapien malesuada, eget pretium justo lacinia.</li>
                            <li>Aliquam ac ipsum auctor, dictum ex vitae, placerat nisi.</li>
                            <li>Suspendisse dictum leo eu nibh pretium, et finibus turpis porta.</li>
                        </ul>


                        <!-- List 3 --> 
                                                <h4 
                            class="px-4 py-4"
                        >
                            Teaching
                        </h4>
                        
                        <ul
                            class="px-16"
                        >
                            <li>Lorem ipsum dolor sit amet, consectetur adipiscing elit</li>
                            <li>Maecenas vehicula purus vitae sapien malesuada, eget pretium justo lacinia.</li>
                            <li>Aliquam ac ipsum auctor, dictum ex vitae, placerat nisi.</li>
                            <li>Suspendisse dictum leo eu nibh pretium, et finibus turpis porta.</li>
                        </ul>

                        <v-btn class="w-100 mt-8 d-flex text-white" style="background-color:#880f0f;">
                            <p class="text-subtitle-2 mr-4"> View More</p>
                            <v-icon icon>mdi-arrow-right-circle</v-icon>
                        </v-btn>
                    </v-card>

                </div>

                <v-card 
                    class="w-50 d-flex flex-column align-center"
                    style="background-color: #D00412;"
                >
                    <h1 class="w-75 text-white">Data Documentation</h1>
                    <p  class="w-75 text-white">per Offices</p>

                    <v-list v-model:opened="open" class="w-75 mt-4" style="background-color:#D00412;">
                        <v-list-item class ="PL_offices_list" append-icon="mdi-arrow-right-circle" title="KSIT Park Development Office"></v-list-item>
                        <v-list-item class ="PL_offices_list" append-icon="mdi-arrow-right-circle" title="ACTION Center"></v-list-item>
                        <v-list-item class ="PL_offices_list" append-icon="mdi-arrow-right-circle" title="Legal Affairs Office"></v-list-item>
                        <v-list-item class ="PL_offices_list" append-icon="mdi-arrow-right-circle" title="Office of the Secretary"></v-list-item>
                        <v-list-item class ="PL_offices_list" append-icon="mdi-arrow-right-circle" title="Office of the Board of Regents"></v-list-item>
                        <v-list-item class ="PL_offices_list" append-icon="mdi-arrow-right-circle" title="Office of Internal Services"></v-list-item>
                        <v-list-item class ="PL_offices_list" append-icon="mdi-arrow-right-circle" title="Presedential Project Management Office"></v-list-item>
                        <v-list-item class ="PL_offices_list" append-icon="mdi-arrow-right-circle" title="Center for Innovation in Engineering Education"></v-list-item>
                        <v-list-item class ="PL_offices_list" append-icon="mdi-arrow-right-circle" title="Office of Culture and Arts"></v-list-item>
                        <v-list-item class ="PL_offices_list" append-icon="mdi-arrow-right-circle" title="Office of Sports"></v-list-item>
                        <v-list-item class ="PL_offices_list" append-icon="mdi-arrow-right-circle" title="Curriculum and Instruction Office"></v-list-item>
                        <v-list-item class ="PL_offices_list" append-icon="mdi-arrow-right-circle" title="Student Affairs and Services Office"></v-list-item>
                        <v-list-item class ="PL_offices_list" append-icon="mdi-arrow-right-circle" title="Testing and Admission Office"></v-list-item>
                    </v-list>
                </v-card>
          
            
        </section>

    </div>
</template>

<style scoped>
    

    #planning_landing{
        display: flex;
        flex-direction: column;
        width: 100%;

    }

    #PL_section_1{
        width: 100%;
        background-image: url('../../../assets/img/bg/bg-2.svg');
 
        height: auto;
        background-size: cover;
        background-position: bottom;
    }
    #PL_section_2{
       
        background-color: white;
        

    }

    #PL_img1{
        position: absolute;
       
        width: 100%;
    }
    #PL_img2{
     
        position: absolute;
        width: 100%;
    }
    #PL_landing_sec2_img{
        
        
    }
    #PL_landing_sec2_img > img{
        width: 50%;
        height: auto;
        /* margin-top: 7rem; */
    }

    #PL_landing_search{
        display: flex;
        background-color: white;
        width: 100%;
        border-radius: 10px;
        align-items: center;
        border: 1px solid rgb(99, 99, 99);
    }

    #PL_landing_search_input{
        width:100%;
        padding: 1rem 2rem;
        border-radius: 10px;
       
    }
    .PL_landing_office_card{
        display: flex;
        align-items: center;
        justify-content: center;
        gap: 20px;
        width:18%;
        padding: 9px 15px;
        border-radius: 20px;
        box-shadow: 14px 15px 14px -9px rgba(0,0,0,0.75);
        -webkit-box-shadow: 14px 15px 14px -9px rgba(0,0,0,0.75);
        -moz-box-shadow: 14px 15px 14px -9px rgba(0,0,0,0.75);
            
    }
    .PL_landing_office_card >  h1{
        display: flex;
        flex-direction: column;
        align-items: center;
        width: 30%;
        line-height: normal;
        color:#B71C1C ;
        font-family: Inter-Bold;
        font-size: 28px;
    }
    .PL_landing_office_card > h1 > span{
        font-family: Inter-Bold;
    }
    .PL_landing_office_card > p{
        width: 60%;
        font-size: 14px;
        font-family: Inter-SemiBold;
        color:#B71C1C ;
        /* border: 1px solid red; */
    }

    #PL_section_4{
        background-image: url(../../../assets/img/bg/bg-4.svg);
        background-position: bottom;
        display: flex; 
        height: 100vh;
        width: 100%;
        background-size: cover;
        padding: 4rem 6rem;

    }

    .PL_offices_list{
        background-color: #D00412;
        color: white;
        border: 1px solid white;
        border-radius: 10px;
        margin-top: 10px;
    }
</style>

<script >
  export default {
    data: () => ({
      open: ['Users'],
    }),
  }
</script>