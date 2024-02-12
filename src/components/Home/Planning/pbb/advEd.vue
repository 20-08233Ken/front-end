<script>

       import AE_OCI from './AE_OCI.vue';
       import AE_OPI from './AE_OPI.vue';


    export default {
        data() {
            return {
            currentComponent: null,
        
            };
        },
        components: {
              AE_OPI,
              AE_OCI

        },
        methods: {
            showComponent(componentName) {
            this.currentComponent = componentName;
           
            }
        }
};
</script>

<template>

        <div>
                <h1 style="color: #b71c1c;font-family: Inter-SemiBold;">Advance Education</h1>

                <div id="indicator_btnCont">
                   <button @click="showComponent('AE_OPI')">Output Indicator</button>
                  <button @click="showComponent('AE_OCI')">Outcome Indicator</button>
                </div>
                <component :is="currentComponent"></component>
        </div>
</template>

<style scoped>

#indicator_btnCont{
    width: 95%;
    align-self: flex-end;
    display: flex;
    gap: 1vw;
    margin: 1vw 0 1vw 3vw;
}

        #indicator_btnCont > button{
               padding: .4vw 1vw;
               border-radius: 5;
               width: 20%;
               background-color: white;
               font-family: Inter-Bold;
               font-size: 15px;
        }
</style>