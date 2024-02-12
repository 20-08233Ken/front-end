
<style scoped>
    @import url('../../../../assets/style/pbb/OCI.css');
</style>

<script setup>

        import OCI_1 from './data_entry/OCI_1.vue';
</script>
<template>
        <div id ="advEd_cont">


            <v-card id ="advEd_card1">

                <div id ="advEd_card1_div1">
                    <span>
                        <v-icon icon style="color: #22af00;font-size: 26px;">mdi-checkbox-marked-circle-outline</v-icon>
                        <p><b> Percentage of graduate students enrolled in research  degree programs</b></p>
                        <OCI_1/>
                        
                    </span>

                    <ol>
                        <li>List graduate programs (with thesis and/or dissertation) in ALL campuses</li>
                        <li> Spell out program name</li>
                        <li>Incomplete entries will be DISREGARDED</li>
                    </ol>    
                    
                    <h4><b>REFERENCE</b> :CHED Memorandum Order No s. 2019,  CMO No.10, s. 2021</h4>
                    <span style="display: flex;width: 100%;">
                        <h4 style="width: 70%;margin-left: 6vw;margin-right: 10px;">MEANS OF VERIFICATION</h4>
                        <ol >
                            <li>Duly certified enrollment list 1st Sem AY 2023-2024</li>
                            <li>For programs claimed as priority but are not listed in CMO 5 s. 2019,  CMO 10 s. 2021, submit RDC or any similar government council resolution/certification that the programs are priority programs</li>
                        </ol>
                    </span>
                </div>

                <div id ="advEd_card1_div2">
                    <span>
                        <v-icon icon style="color: #22af00;font-size: 26px;">mdi-checkbox-marked-circle-outline</v-icon>
                        <p> <b>Percentage of accredited graduate Programs</b></p>
                        <OCI_1/>
                    </span>

                    <ol>
                        <li>List graduate programs by Campus</li>
                        <li>Choose ACCREDITATION STATUS (tick ONE from column A-F)</li>
                        <li>Please indicate period of validity, including programs with CANDIDATE STATUS (CS)</li>
                        <li>For programs that are NOT ACCREDITED (NA), indicate the reason for non-accreditation in column 5. Choose from drop-down list; Programs with expired accreditation need </li>
                        <li>Incomplete entries will be DISREGARDED</li>
                    </ol>

                    <p><b>MEANS OF VERIFICATION:</b> Accreditation certificates; if certificates are not available, AACCUP letter/notice/resolution of accredited programs</p>
                </div>

                <!-- <div id ="advEd_card1_div3">
                    <span>
                        <v-icon icon style="color: #22af00;font-size: 26px;">mdi-checkbox-marked-circle-outline</v-icon>
                        <p><b>Percentage of graduate school faculty engaged in research work</b></p>
                        <OCI_1/>
                    </span>
                    
                    <ol>
                        <li> List undergraduate programs in ALL campuses</li>
                        <li>Choose ACCREDITATION LEVEL/STATUS (tick ONE from column A-F)</li>
                        <li>Please indicate period of validity, including programs with CANDIDATE STATUS (CS), VALIDITY PERIOD AS OF DECEMBER 31, 2023</li>
                        <li>For programs that are NOT ACCREDITED (NA), indicate the reason for non-accreditation in column 5. Choose from drop-down list</li>
                        <li>Incomplete entries will be DISREGARDED</li>
                    </ol>       

                    <p><b>MEANS OF VERIFICATION:</b> Accreditation certificates; if certificates are not available, AACCUP letter/notice/resolution of accredited programs</p>
                    
                </div> -->
            </v-card>

            <button id ="advEd_submitBtn">Submit</button>
        </div>
</template>