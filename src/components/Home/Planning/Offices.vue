<style scoped>
    @import url('../../../assets/style/offices.css');
</style>

<script>
    import Header from '../Header.vue';
    import Footer from '../footer.vue'

  
  export default {
    data: () => ({
      OUP: [
        { title: 'KSIT Park Development Office' },
        { title: 'Action Cente' },
        { title: 'Office of the Secretary' },
        { title: 'Office of the Board of Regents' },
        { title: 'Internal Audit Services Office' },
        { title: 'Presidential Project Management Office' },
        { title: 'Center for Innovation in Engineering Education' },
        { title: 'Legal Affairs Office'}
      ],
      OVPAA: [
        { title: 'Office of Culture and Arts' },
        { title: 'Office of Sports' },
        { title: 'Office of Curriculum and Instructions' },
        { title: 'Office of Student Affairs and Services' },
        { title: 'Scholarship Office' },
        { title: 'Testing and Admission Office' },
        { title: 'Center for Transformative Learning ' },
        { title: 'Office of Quality Assurance Management'}
      ],
      OVPRDE: [
        { title: 'Office of Research, Development, and Extension Services' },
        { title: 'Office of Industry, Energy and Emerging Technology Research' },
        { title: 'Office of Agriculture, Aquatic, and Natural Resources Research' },
        { title: 'Office of Integrated Basic and Applied Research' },
        { title: 'Research Management Office' },
        { title: 'Research Publication Management Office' },
        { title: 'Knowledge and Technology Transfer Management Office ' },
        { title: 'Extension Services Office'},
        { title: 'Community Development Office ' },
        { title: 'Extension Monitoring and Impact Assessment Office  ' },
        { title: 'Gender and Development Advocacies Office ' },
        { title: 'Management and Health Research Office' },
        { title: 'STEER Hub' },
      ],
      OVPAF: [
        { title: 'Office of Administration and Impact Assessment' },
        { title: 'Office of Administration Services' },
        { title: 'Human Resource Management Office ' },
        { title: 'Finance Services Office' },
        { title: 'Accounting Office ' },
        { title: 'Budget Office' },
        { title: 'Procurement Office' },
        { title: 'Records Office'},
        { title: 'General Services Office' },
        { title: 'Cashiering Office  ' },
        { title: 'Project Management Office'},
        { title: 'Health Services Office ' },
        
      ],
      OVPDE: [
        { title: 'Development and  External Services Office ' },
        { title: 'ICT Service Office ' },
        { title: 'Network and Systems Administration Services Office' },
        { title: 'ICT Special Project Office ' },
        { title: 'Electronic System Research Center Office' },
        { title: 'GIS Application Development Center' },
        { title: 'External Affairs ' },
        { title: 'Auxiliary Services Office'},
        { title: 'Digital Transformation Center' },
        { title: 'Manufacturing Research Center' },
        { title: 'ICT Operations Office '},
        { title: 'Institutional Planning and Development Office' },
        
        { title: 'ICT Operations Office ' },
        { title: 'Material Testing and Calibration Center' },
        { title: 'Analytical Research Center Office' },
        { title: 'Food Innovation Center' },
        { title: 'Social Innovation Research Center' },

        { title: 'Management Information System Office' },
        { title: 'Center for Technopreneurship and Innovation' },
        { title: 'VIP Corals Office - Lobo' },
        { title: 'VIP Corals Office - Nasugbu' },
      ],
    }),
    components:{
        Header
    }
  }

</script>

<template>
    <main id ="PL_offices_main">
            <Header/>

            <section id ="PL_offices_sec1"> 
                <span>
                    <h1>Report Submission</h1>
                    <p>Submit report in CSV File with proper documentation and format of data</p>
                    
                    <span  id="PL_offices_sec1_search">
                        <input type="search" name="" placeholder="Search for an office">
                        <v-icon icon>mdi-magnify</v-icon>
                    </span>
                
                </span>
                <span>
                    <img src="" alt="Image heere">
                </span>
            </section>

            <section id ="PL_offices_sec2">

                <h2>Head Offices</h2>
                <p>Find your Office under these head offices</p>

                <div>

                    <v-menu >
                        <template v-slot:activator="{ props }">
                            <v-btn
                                class="PL_offices_card1"
                                v-bind="props"
                            >
                            Office of the University President
                            </v-btn>
                        </template>
                        <v-list>
                            <v-list-item
                            v-for="(item, index) in OUP"
                            :key="index"
                            :value="index"
                            >
                            <v-list-item-title>{{ item.title }}</v-list-item-title>
                            </v-list-item>
                        </v-list>
                    </v-menu>


                    <v-menu>
                        <template v-slot:activator="{ props }">
                            <v-btn
                                class="PL_offices_card1"
                                v-bind="props"
                            >
                            Office of the Vice President for Academic Affairs
                            </v-btn>
                        </template>
                        <v-list>
                            <v-list-item
                            v-for="(item, index) in OVPAA"
                            :key="index"
                            :value="index"
                            >
                            <v-list-item-title>{{ item.title }}</v-list-item-title>
                            </v-list-item>
                        </v-list>
                    </v-menu>

                    <v-menu>
                        <template v-slot:activator="{ props }">
                            <v-btn
                                class="PL_offices_card1"
                                v-bind="props"
                            >
                            Office of the Vice President for Research, Development, and Extension Services
                            </v-btn>
                        </template>
                        <v-list>
                            <v-list-item
                            v-for="(item, index) in OVPRDE"
                            :key="index"
                            :value="index"
                            >
                            <v-list-item-title>{{ item.title }}</v-list-item-title>
                            </v-list-item>
                        </v-list>
                    </v-menu>

                    <v-menu>
                        <template v-slot:activator="{ props }">
                            <v-btn
                                class="PL_offices_card1"
                                v-bind="props"
                            >
                            Office of the Vice President for Administration and Finance
                            </v-btn>
                        </template>
                        <v-list>
                            <v-list-item
                            v-for="(item, index) in OVPAF"
                            :key="index"
                            :value="index"
                            >
                            <v-list-item-title>{{ item.title }}</v-list-item-title>
                            </v-list-item>
                        </v-list>
                    </v-menu>           


                    <v-menu>
                        <template v-slot:activator="{ props }">
                            <v-btn
                                class="PL_offices_card1"
                                v-bind="props"
                            >
                            Office of the Vice President for Development and External Affiars
                            </v-btn>
                        </template>
                        <v-list>
                            <v-list-item
                            v-for="(item, index) in OVPDE"
                            :key="index"
                            :value="index"
                            >
                            <v-list-item-title>{{ item.title }}</v-list-item-title>
                            </v-list-item>
                        </v-list>
                    </v-menu>      

    
                </div>

            </section>
<!-- 
            <section id ="PL_offices_sec3">

                <div>
                    <span></span>
                        <h5>Office of the University President</h5>
                    <span></span>
                </div>

                <div>

                    <v-card class="PL_offices_card2">KSIT Park Development Office</v-card>
                    <v-card class="PL_offices_card2">Action Center</v-card>
                    <v-card class="PL_offices_card2">Office of the Secretary</v-card>
                    <v-card class="PL_offices_card2">Office of the Board of Regents</v-card>
                    <v-card class="PL_offices_card2">Internal Audit Services Office</v-card>
                    <v-card class="PL_offices_card2">Presidential Project Management Office</v-card>
                    <v-card class="PL_offices_card2">Center for Innovation in Engineering Education</v-card>
                    <v-card class="PL_offices_card2">Legal Affairs Office</v-card>

                </div>

            </section>





            <section id ="PL_offices_sec4">

                <div>
                    <span></span>
                        <h5>Office of the Vice President for Academic Affairs</h5>
                    <span></span>
                </div>

                <div>

                    <v-card class="PL_offices_card3">Office of Culture and Arts </v-card>
                    <v-card class="PL_offices_card3">Office of Sports </v-card>
                    <v-card class="PL_offices_card3">Office of Curriculum and Instructions </v-card>
                    <v-card class="PL_offices_card3">Office of Student Affairs and Services  </v-card>
                    <v-card class="PL_offices_card3">Scholarship Office  </v-card>
                    <v-card class="PL_offices_card3">Testing and Admission Office  </v-card>
                    <v-card class="PL_offices_card3">Center for Transformative Learning </v-card>
                    <v-card class="PL_offices_card3">Office of Quality Assurance Management  </v-card>
                </div>

            </section>

            <section id ="PL_offices_sec5">

                <div>
                    <span></span>
                        <h5>Office of the Vice President for Research, Development, and Extension Services</h5>
                    <span></span>
                </div>

                <div>

                    <v-card class="PL_offices_card4">Office of Research, Development, and Extension Services</v-card>
                    <v-card class="PL_offices_card4">Office of Industry, Energy and Emerging Technology Research</v-card>
                    <v-card class="PL_offices_card4">Office of Agriculture, Aquatic, and Natural Resources Research </v-card>
                    <v-card class="PL_offices_card4">Office of Integrated Basic and Applied Research </v-card>
                    <v-card class="PL_offices_card4">Research Management Office </v-card>
                    <v-card class="PL_offices_card4">Research Publication Management Office </v-card>
                    <v-card class="PL_offices_card4">Knowledge and Technology Transfer Management Office </v-card>
                    <v-card class="PL_offices_card4">Extension Services Office </v-card>
                    <v-card class="PL_offices_card4">Community Development Office  </v-card>
                    <v-card class="PL_offices_card4">Extension Monitoring and Impact Assessment Office  </v-card>
                    <v-card class="PL_offices_card4">Gender and Development Advocacies Office  </v-card>
                    <v-card class="PL_offices_card4">Management and Health Research Office  </v-card>
                    <v-card class="PL_offices_card4">STEER Hub </v-card>
                </div>

            </section>


            <section id ="PL_offices_sec6">

                <div>
                    <span></span>
                        <h5>Office of the Vice President for Administration and Finance</h5>
                    <span></span>
                </div>

                <div>

                    <v-card class="PL_offices_card5">Office of Administration and Impact Assessment </v-card>
                    <v-card class="PL_offices_card5">Office of Administration Services </v-card>
                    <v-card class="PL_offices_card5">Human Resource Management Office  </v-card>
                    <v-card class="PL_offices_card5">Finance Services Office </v-card>
                    <v-card class="PL_offices_card5">Accounting Office </v-card>
                    <v-card class="PL_offices_card5">Budget Office  </v-card>
                    <v-card class="PL_offices_card5">Procurement Office  </v-card>
                    <v-card class="PL_offices_card5">Records Office  </v-card>
                    <v-card class="PL_offices_card5">General Services Office   </v-card>
                    <v-card class="PL_offices_card5">Cashiering Office  </v-card>
                    <v-card class="PL_offices_card5">Project Management Office   </v-card>
                    <v-card class="PL_offices_card5">Health Services Office  </v-card>
                    
                </div>

            </section>

            <section id ="PL_offices_sec7">

                <div>
                    <span></span>
                        <h5>Office of the Vice President for Administration and Finance</h5>
                    <span></span>
                </div>

                <div>

                    <v-card class="PL_offices_card6">Development and  External Services Office </v-card>
                    <v-card class="PL_offices_card6">ICT Service Office  </v-card>
                    <v-card class="PL_offices_card6">Network and Systems Administration Services Office   </v-card>
                    <v-card class="PL_offices_card6">ICT Special Project Office  </v-card>
                    <v-card class="PL_offices_card6">Electronic System Research Center Office </v-card>
                    <v-card class="PL_offices_card6">GIS Application Development Center </v-card>
                    <v-card class="PL_offices_card6">External Affairs </v-card>
                    <v-card class="PL_offices_card6">Auxiliary Services Office</v-card>
                    <v-card class="PL_offices_card6">Digital Transformation Center   </v-card>
                    <v-card class="PL_offices_card6">Manufacturing Research Center  </v-card>
                    <v-card class="PL_offices_card6">ICT Operations Office    </v-card>
                    <v-card class="PL_offices_card6">Institutional Planning and Development Office </v-card>

                    <v-card class="PL_offices_card6">ICT Operations Office  </v-card>
                    <v-card class="PL_offices_card6">Material Testing and Calibration Center  </v-card>
                    <v-card class="PL_offices_card6">Analytical Research Center Office  </v-card>
                    <v-card class="PL_offices_card6">Food Innovation Center</v-card>
                    <v-card class="PL_offices_card6">Social Innovation Research Center  </v-card>
                    
 
                    <v-card class="PL_offices_card6">Management Information System Office </v-card>
                    <v-card class="PL_offices_card6">Center for Technopreneurship and Innovation</v-card>
                    <v-card class="PL_offices_card6">VIP Corals Office - Lobo</v-card>
                    <v-card class="PL_offices_card6">VIP Corals Office - Nasugbu</v-card>
                                  
                </div>
            </section> -->


            <section style="width: 100%;">
                
                    <!-- <Footer/> -->
            </section>
    </main>
</template>