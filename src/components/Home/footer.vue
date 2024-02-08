<template>
    <div class="w-100 d-flex" style="background-color: #F5F5F5;">
        <h1 
            class="w-50 text-white" 
            style="padding:  3rem 0 0 6vw; background-color: #D00412; clip-path: polygon(0 0, 95% 0, 100% 100%, 0% 100%);    font-size: clamp(18px,5vw,40px);">
            University Dataset
        </h1>
    </div>
    <section 
           
            id ="footer_container"

        >
                <div>
                  <!-- Card 1 -->  
                    <v-card id ="card_1"  style="border-radius: 10px; border:1px solid white;">
                        <h3 
                            class="w-100 d-flex align-center justify-space-evenly text-white py-4"
                            style="background-color: #94080D;">
                            <img 
                                src="../../assets/img/qs-stars.png"
                                style="width: 18%;height: auto;"
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
                    <v-card id ="card_1"  style="border-radius: 10px; border:1px solid white;">
                        <h3 
                            class="w-100 d-flex align-center justify-space-evenly text-white py-4"
                            style="background-color: #94080D;">
                            <img 
                                src="../../assets/img/qs-stars.png"
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

                <v-card id="card_3">
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
</template>


<style scoped>
    .PL_offices_list{
        background-color: #D00412;
        color: white;
        border: 1px solid white;
        border-radius: 10px;
        margin-top: 10px;
    }

    #footer_container{
        width: 100%;
        display: flex;
        align-items: center;
        background-color: #D00412;  
    }

    #footer_container > div:first-child{
        width: 50%;
        display: flex;
        align-items: center;
        background-color: #D00412; 
        margin-top: 8vh; 
        gap: 3em;
        margin-left: 5vw;
    }

    #card_3{
        width: 50%;
        display: flex;
        flex-direction: column;
        align-items: center;
        background-color: #D00412
    }
    li{
        font-size: clamp(10px,2vw,14px);
    }
    h4{
        font-size: clamp(14px,3vw,18px);
    }


    @media (max-width:1024px){
        #footer_container{
            flex-direction: column;

        }
        #card_1{
            width: 50%;
        }
        #card_3{
        width:100%;
        margin-top: 8vh;

    }

        #footer_container > div:first-child{
        width: 90%;

        }
    }

    @media (max-width:768px){
        #footer_container > div:first-child{
            flex-direction: column;
            gap: 4em;
            width: 100%;
        }

        #card_1{
            width: 80%;
        }

    }

</style>
<script >
  export default {
    data: () => ({
      open: ['Users'],
    }),
  }
</script>