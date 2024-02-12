<script setup>

    import Header from '../Header.vue';

</script>

<style scoped>
    @import url('../../../assets/style/dataset.css');
</style>

<template>

    <main id ="PL_dataset_main">
        <Header/>

        <div id ="PL_dataset_submain">

           <span id ="PL_dataset_span1">
                <h1>Dataset</h1>
                <p>Contains documentation of data being regulated within the
                    Management Information System (MIS) Office
                </p>

                <v-card id="PL_dataset_card1">
                        <h2>Office of Human Resource</h2> 
                        <ul>
                            <li>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</li>
                            <li>Maecenas vehicula purus vitae sapien malesuada, eget pretium justo lacinia.</li>
                            <li>Aliquam ac ipsum auctor, dictum ex vitae, placerat nisi.</li>
                            <li>Suspendisse dictum leo eu nibh pretium, et finibus turpis porta.</li>
                            <li>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</li>
                            <li>Maecenas vehicula purus vitae sapien malesuada, eget pretium justo lacinia.</li>
                            <li>Aliquam ac ipsum auctor, dictum ex vitae, placerat nisi.</li>
                            <li>Suspendisse dictum leo eu nibh pretium, et finibus turpis porta.</li>
                            <li>Duis fringilla massa nec dapibus laoreet.</li>
                            <li>Donec hendrerit ligula id diam consectetur, quis facilisis quam pretium.</li>
                            <li>Cras euismod tortor at felis auctor, commodo cursus nibh elementum.</li>
                            <li>Donec non elit at magna pretium aliquam in in diam.</li>
                            <li>Vestibulum ullamcorper mi et felis tempus, quis rutrum est tristique.</li>
                            <li>Nam vitae orci vehicula, ornare ante sit amet, laoreet purus.</li>
                       
                        </ul>
                </v-card>

           </span> 

           <span  id ="PL_dataset_span2">

                <div>
                    <input type="search" id="gsearch" name="gsearch" placeholder="Search for an office">
                    <v-icon icon>mdi-magnify</v-icon>
                </div>
                <v-card id="PL_dataset_card2" elevation ="0">
                    <v-list v-model:opened="open" style="background-color: #F5F5F5;">
                        <v-list-item class ="PL_dataset_list" append-icon="mdi-arrow-right-circle" title="KSIT Park Development Office"></v-list-item>
                        <v-list-item class ="PL_dataset_list" append-icon="mdi-arrow-right-circle" title="ACTION Center"></v-list-item>
                        <v-list-item class ="PL_dataset_list" append-icon="mdi-arrow-right-circle" title="Legal Affairs Office"></v-list-item>
                        <v-list-item class ="PL_dataset_list" append-icon="mdi-arrow-right-circle" title="Office of the Secretary"></v-list-item>
                        <v-list-item class ="PL_dataset_list" append-icon="mdi-arrow-right-circle" title="Office of the Board of Regents"></v-list-item>
                        <v-list-item class ="PL_dataset_list" append-icon="mdi-arrow-right-circle" title="Office of Internal Services"></v-list-item>
                        <v-list-item class ="PL_dataset_list" append-icon="mdi-arrow-right-circle" title="Presedential Project Management Office"></v-list-item>
                        <v-list-item class ="PL_dataset_list" append-icon="mdi-arrow-right-circle" title="Center for Innovation in Engineering Education"></v-list-item>
                        <v-list-item class ="PL_dataset_list" append-icon="mdi-arrow-right-circle" title="Office of Culture and Arts"></v-list-item>
                        <v-list-item class ="PL_dataset_list" append-icon="mdi-arrow-right-circle" title="Office of Sports"></v-list-item>
                        <v-list-item class ="PL_dataset_list" append-icon="mdi-arrow-right-circle" title="Curriculum and Instruction Office"></v-list-item>
                        <v-list-item class ="PL_dataset_list" append-icon="mdi-arrow-right-circle" title="Student Affairs and Services Office"></v-list-item>
                        <v-list-item class ="PL_dataset_list" append-icon="mdi-arrow-right-circle" title="Testing and Admission Office"></v-list-item>
                    </v-list>
                </v-card>

           </span>
        </div>
    </main>
</template>