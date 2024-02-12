<template>
        <div >
            <v-toolbar class=" w-100 d-flex bg-red-darken-3 pa-2 w-100 py-3">
                        <v-btn class="ml-10">
                            <v-icon icon="mdi-menu"/>
                        </v-btn>
                        <img id ="univ-logo" src="../../assets/img/school.png" alt="">

                        <v-btn>
                            <router-link to="/" style="text-decoration: none;" class="text-white">
                                University MIS
                            </router-link>
                        </v-btn>
                        

                        
                        <span class="w-100 " id ="nav-list">
                            <ul class="w-50 mx-10 d-flex justify-space-around text-subtitle-1"  style="list-style-type: none;">
                                <li class="py-3" ><router-link to ="/landing"  style="text-decoration: none; color: white"> Profile</router-link></li>
                                <li> <router-link to ="/dashboard"  style="text-decoration: none; color: white"> Dashboard </router-link></li>
                                <li><router-link to ="/dataset"  style="text-decoration: none; color: white">Dataset </router-link></li>
                                <li><router-link to ="/pbb"  style="text-decoration: none; color: white">PBB</router-link></li>
                                <li><router-link to ="/offices"  style="text-decoration: none; color: white">Offices</router-link></li>
                                
                            </ul>
                        </span>
            </v-toolbar>
        </div>
</template>


<style>

    
    #univ-logo{
        width: 3%;
        height: auto;
    }

    #nav-list > ul > li{
        display: flex;
        align-items: center;
        justify-content: center;

        padding: 1rem 2rem;
        width: 20%;
    }
    #nav-list > ul > li:hover{
        background-color: #B71C1C;
    }
</style>