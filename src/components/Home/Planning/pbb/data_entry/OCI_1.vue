<template>
           <div class="text-center" >
                                <v-btn
                                id ="dataEntry"
                                >
                                Data Entry

                                <v-dialog
                                    v-model="dialog"
                                    activator="parent"
                                    width="auto"
                                >
                                    <v-card>
                                    <v-card-text>
                                        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
                                    </v-card-text>
                                    <v-card-actions>
                                        <v-btn color="primary" block @click="dialog = false">Close Dialog</v-btn>
                                    </v-card-actions>
                                    </v-card>
                                </v-dialog>
                                </v-btn>
                            </div>
</template>


<script>
  export default {
    data () {
      return {
        dialog: false,
      }
    },
  }
</script>

<style scoped>
       #dataEntry
            {
            display: flex;
            align-items: center;
            justify-content: center;
            background-color: #B71C1C;
            border-radius: 20px;
            color: white;
            padding: .4vw 1vw;
            font-size: 14px;
            width: 70%;
            margin-left: 4vw; 
            font-family: Inter-Regular;
            font-size: 14px;
                    }
</style>
