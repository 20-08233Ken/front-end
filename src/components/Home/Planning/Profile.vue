<template>
    <div class="d-flex w-100" >
        <section id ="profile-left" class=" pt-8" style="width: 75%;">

            <div class="pl-14">
            <span class="d-flex align-center w-100 justify-space-between">
                <h1 class="text-red-darken-4">
                    OFFICE OF 
                </h1>

                <v-btn class="text-none mr-8 rounded-circle" color="red-darken-4" elevation="0" stacked>
                    <v-badge content="2" color="error">
                        <v-icon>mdi-bell-outline</v-icon>
                    </v-badge>
                </v-btn>

            </span>
            <p>Campus-Central</p>

            <h4 class="mt-4">Submissions</h4>

            <div class="mt-2 d-flex w-100">

                <v-card class="d-flex align-center py-4 px-4 rounded-lg mr-10" style="width: 22%;">
                    <h1 class="mr-4 text-red-darken-4">QPRO</h1>
                    <p>Quarterly</p>
                </v-card>

                <v-card class="d-flex align-center py-4 px-4 rounded-lg" style="width: 22%;">
                    <h1 class="mr-4 text-red-darken-4">PBB</h1>
                    <p>Performance-based Bonus (Q3)</p>
                </v-card>
            </div>

            <h4 class="mt-6 text-red-darken-4">Performance Statistics</h4>

            <div id ="graph-cont-1" class="d-flex w-100" >

                <span style="width: 30%;" >
                    <img src="../../../assets/img/graph/g3.png" alt="" >
                    Completion of Overall Data
                </span>

                <span style="width: 30%;" >
                    <img src="../../../assets/img/graph/g2.png" alt="">
                    PBB-Grading: Non-Eligible
                </span>

                <span style="width: 30%;">
                    
                    <img src="../../../assets/img/graph/g1.png" alt="" style="width: 75%;">
                    2023
                </span>
            </div>
        </div>

        <div class="w-100 px-8 py-3 text-white " style="background-color: #B71C1C;">
                MIS Office Summary of Data
            </div>
            <div>

                <v-table class="w-100">
                    <thead>
                        <tr style="background-color: #FFEBEE;">
                            <th class ="w-25 text-center"> Data Title / Name</th>
                            <th class ="w-75 text-center"> Description</th>
                        </tr>
                        <tr style="background-color: white;">
                            <td></td>
                            <td></td>
                        </tr>
                        <tr style="background-color: white;">
                            <td></td>
                            <td></td>
                        </tr>
                        <tr style="background-color: white;">
                            <td></td>
                            <td></td>
                        </tr>
                        
                    </thead>
                </v-table>
            </div>
        </section>

        <section id ="profile-right" style="width:25%;background-color: white;">

            <div 
                style="height: 20rem; border:"
                class="d-flex justify-center align-center"
            >
                Calendar
            </div>
            <div class="d-flex flex-column px-6 py-5">
              <h4 class="w-100  text-red-darken-4">Activities</h4>

              <ul style="list-style-type: none;">

                <li class="d-flex align-center mt-5">
                    <span 
                        class="py-4 d-flex justify-center align-center text-white mr-4"
                        style="background-color: #B71C1C; width:3rem;height:3rem;border-radius: 50%;">
                        PBB
                    </span>
                    <p class="d-flex flex-column">
                        Submission of PBB Documents
                        <span class="text-subtitle-2 text-grey-darken-1">July 21, 2023</span>
                    </p>
                </li>

                <li class="d-flex align-center mt-7">
                    <span 
                        class="py-4 d-flex justify-center align-center text-white mr-4"
                        style="background-color: #B71C1C; width:3rem;height:3rem;border-radius: 50%;">
                        PBB
                    </span>
                    <p class="d-flex flex-column">
                        Submission fpr the office data
                        <span class="text-subtitle-2 text-grey-darken-1">July 28, 2023</span>
                    </p>
                </li>
            
                <li class="d-flex align-center mt-7">
                    <span 
                        class="py-4 d-flex justify-center align-center text-white mr-4"
                        style="background-color: #B71C1C; width:3rem;height:3rem;border-radius: 50%;">
                        PBB
                    </span>
                    <p class="d-flex flex-column">
                        Submission of of OPCR: Third Quarter
                        <span class="text-subtitle-2 text-grey-darken-1">July 28, 2023</span>
                    </p>
                </li>
              </ul>
            </div>

        </section>
    </div>
</template>

<style scoped>

    #graph-cont-1 > span{
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
  
        padding: 2rem 1rem;
    
        
    }
    #graph-cont-1 > span > img{
  
        width: 56%;
        
    }

    td > span{
        /* border: 1px solid red; */
    }

    th{
        border-right: 1px solid black;
    }

</style>