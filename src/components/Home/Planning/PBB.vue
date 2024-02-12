<script>
    import Header from '../header.vue';
    import OPI from './pbb/OPI.vue'
    import OCI from './pbb/OCI.vue'
    import researchServices from './pbb/researchServices.vue'
    import techAdvisory from './pbb/techAdvisory.vue';
    import higherEd from './pbb/higherEd.vue';
    import advEd from './pbb/advEd.vue'

    export default {
        data() {
            return {
            currentComponent: null,
        
            };
        },
        components: {
            OPI,
            OCI,
            Header,
            researchServices,
            techAdvisory,
            higherEd,
            advEd
            // Button3
        },
        methods: {
            showComponent(componentName) {
            this.currentComponent = componentName;
           
            }
        }
};
</script>

<style scoped>
    @import url('../../../assets/style/pbb.css');
</style>

<template>
    <main>
        <Header/>

        <header>
            <div>
                <h1 style="color:#B71C1C;font-family: Inter-Bold;font-size: 40px;">Peformance-Based Bonus</h1>
                <h5 style="font-family: Inter-Bold;font-size: 16px;">Current Quarter: Q1</h5>
                <h5 style="font-family: Inter-Regular;font-size: 14px;">FY 2023</h5>
            </div>

            <div>   
                <button id="pb_db_bttn">Status dashboard</button>
                <button id="pb_submit_bttn">Submit</button>
            </div>
        </header>

        <section id ="pbb_sec1">
            <aside>
                
                <p class="pbb_sideTitle">Peformance Results</p>
                <ul>
                    <li><button @click="showComponent('higherEd')">Higher Education</button></li>
                    <li><button @click="showComponent('advEd')">Advanced Education</button></li>
                    <li><button @click="showComponent('researchServices')">Research Services</button></li>
                    <li><button @click="showComponent('techAdvisory')">Technical Advisory Extension</button></li>
                </ul>

                <p class="pbb_sideTitle">Process Results</p>
                <ul>
                    <li>Higher Education</li>
                    <li>Advanced Education</li>
                    <li>Research Services</li>
                    <li>Technical Advisory Extension</li>
                </ul>

                <p  class="pbb_sideTitle">Financial Results</p>
                <ul>
                    <li>Modified Form A for SUC’s Performance Report</li>
                </ul>

                <p  class="pbb_sideTitle">Citizen Client Satisfaction Results</p>
                <ul>
                    <li>Citizen / Client Satisfaction Report </li>
                    <li>Summary Report of Complaints Received through #8888 Hotline</li>
                    <li>Forms 1.0</li>
                </ul>

                <p class="pbb_sideTitle">Agency Accountabilities</p>
                <ul>
                    <li>Updating of Transparency Seal</li>
                    <li>Compliance with the Freedom of Information (FOI) Program</li>
                    <li>Updating of Citizen’s or Service Charter </li>
                    <li>Compliance to Audit Findings and Liquidation of Cash Advances</li>
                    <li>Submission and Review of SALN </li>

                    <li>PhilGEPS posting of all invitations to bids and awarded contracts </li>
                    <li>Submission of FY 2022 Annual Procurement Plan-Common Use Supplies and Equipment (APP-CSE) </li>
                    <li>Undertaking of Early Procurement Activities covering 2022 Procurement Projects </li>
                </ul>

            </aside>
            
            <div>
                <component :is="currentComponent"></component>

            </div>
        </section>
    </main>
</template>