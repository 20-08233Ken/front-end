<script setup>
    import Graph1 from './graph/graph1.vue';
    import Graph2 from './graph/graph2.vue';
    import Graph3 from './graph/graph3.vue';
    import Footer from '../footer.vue';
    import Header from '../header.vue';
</script>

<style scoped>
    @import url(../../../assets/style/landing.css);
    @import url(../../../assets/style/responsive_landing.css);
</style>

<template>
    <Header/>
    <div id ="PL_landing_main">
        
        
        <section id ="PL_landing_sec1">

            <!-- Sub Container 1 -->
            <div>
                <span id="PL_landing_sec1_p1">
                    <h1>University Management</h1>
                    <h1 style="color:#EC061D">Information<span style ="margin: 0 0 0 .3em;color: #B71C1C;">System</span></h1>
                    <p>Central System for Managing and Processing Data of Batangas State University</p>
                    <p>
                        Lorem ipsum dolor sit amet consectetur adipisicing elit. Illo quidem placeat veritatis
                        accusantium laborum dignissimos animi? Maiores labore ducimus distinctio vero a fugiat
                        autem dolore optio sapiente magnam! Veniam, at.
                        accusantium laborum dignissimos animi? Maiores labore ducimus distinctio vero a fugiat
                        autem dolore optio sapiente magnam! Veniam, at.
                    </p>
                </span>

                <span id="PL_landing_sec1_p2">
                    <img src="../../../assets/img/merge/img1.png" alt="">
                </span>
            </div>

            <!-- Sub Container 2 and 3-->
            <h1>Search for an Office</h1>
            <div>
                <span id ="PL_landing_search" >
                    <input type="text" name="" id="PL_landing_search_input" placeholder="Seacrch">
                    <v-btn elevation="0" style="width: 2%;">
                            <v-icon icon>mdi-magnify</v-icon>
                    </v-btn>
                </span>
            </div>
            <!-- Sub Container 4 and 5 -->
            <h1>Head Offices</h1>
            <p>Find your Office under these head offices</p>

            <!-- Sub Container 6 -->
            <div>
                    <span class="w-100 d-flex justify-space-evenly">
                        <v-card class="PL_landing_office_card">
                            <h1>OUP</h1>
                            <p >Office of the University President</p>
                        </v-card>

                        <v-card class="PL_landing_office_card">
                            <h1>OVP <span>AA</span></h1>
                            <p>Office of the Vice President for Academic Affairs</p>
                        </v-card>

                        <v-card class="PL_landing_office_card">
                            <h1>OVP <span>RDES</span></h1>
                            <p>Office of the Vice President for  Research, Development, and Extension Services</p>                          
                        </v-card>

                        <v-card class="PL_landing_office_card">
                            <h1>OVP <span>AF</span></h1>
                            <p>Office of the Vice President for  Administration and Finance</p>           
                        </v-card>

                        <v-card class="PL_landing_office_card">
                            <h1 style="font-family: 'Roboto';">OVP <span>DEA</span></h1>
                            <p>Office of the Vice President for Development and External  Affairs</p>                          
                        </v-card>
                    </span>
            </div>

            <div>
                    <v-btn class="text-white rounded-lg">See more Offices</v-btn>
            </div>

                
        </section>

        <section id="PL_section_2">
                <div>
                    <span>
                        <h1>University Data</h1>
                        <h1>Dashboard</h1>
                        <p>Monitor overall data gathered within the university. Process those data and visualize those data into more understandable presentation.</p>
                        <p>Help visualize the trajectory of the university through visualizing data from criterion of different university rankings.</p>
                    </span>
                    
                    <span>
                        <Graph1/>
                        <Graph2/>
                    </span>
                </div>
                <div>
                    <Graph3/>
                </div>

                <div>
                    <v-btn class="text-white rounded-lg">
                        View more in Dashboard
                    </v-btn>
                </div>

        </section>

        <section id ="PL_section_3">

            <div>
                <span>
                    <span>
                        <h1>University <span style="color: #EC061D;font-family: Inter-bold;">Facts</span></h1>
                        <h1>and <span style="color: #EC061D;font-family: Inter-bold;">Figures</span></h1>
                    </span>

                    <p style="width: 70%;margin-top: 4vh;"> View the university’s facts and information coming from data gathered within the whole school year.</p>
                    <p style="width: 70%;margin-top: 2vh;">Showcase the capabilities of the university through organized report and data visualization</p>
               
                    
                    <button id ="PL_section_3_dlBttn"> 
                        <img src="../../../assets/img/icons8-pdf-50.png" alt="" style="max-width: 2rem;margin-right: 1em;">
                        <p style=" font-size: clamp(10px,2vw,14px);">Download BatStateU Facts and Figures</p>
                    </button>

                    <p style="margin-top: 2vh;width: 70%;text-align: center;font-size: clamp(10px,2vw,14px);"> <u> View University Facts and Figures Table of Contents</u></p>
               
                </span>

                <span>
                    <img src="../../../assets/img/dash.png" alt="" style="max-width: 65%;width: 100%;">
                </span>
            </div>

        </section>

        <section>

            <Footer/>

        </section>
    </div>
</template>


<script >
  export default {
    data: () => ({
      open: ['Users'],
    }),
  }
</script>