<style >
    @import url('../styles/home.css');
</style>

<script setup>
   import Header from "../components/Home/Header.vue"
   import Subnav2 from "../components/Home/Subnav2.vue";
    import Landing from "../components/Home/Dean/Landing.vue";

    import PlanningProfile from '../components/Home/Planning/Profile.vue'
</script>

<template>
    <div id = "home-main">
        <Header></Header>
        <PlanningProfile/>

            </div>
    
</template>


<style scoped>
    #home-main{
        width: 100%;
       
    }


</style>