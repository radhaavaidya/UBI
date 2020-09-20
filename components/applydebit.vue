<template>

  <v-card
    class="mx-auto"
    max-width="400">

    <v-img
      class="mx-auto"
      height="300px"
      src="icons-01.jpg">
    </v-img>
      <!-- src is the link of the image in the static -->
       <v-card-text class="text--primary">
       </v-card-text>

    <v-card-actions>
      <v-dialog v-model="dialog" persistent max-width="420">
        <template v-slot:activator="{ on, attrs }">
          <v-btn
            color="primary"
            dark
            v-bind="attrs"
            v-on="on">
            Apply for online debit card
          </v-btn> 
        </template>
        <v-card>
           <v-card-title 
             class="headline">
             If you already have an active debit card, Please do not apply for debit card online
           </v-card-title>
          <!-- v-modal dialog is the mode/dialog pop up with width 420-->
          <!-- v-bind and v-on helps in opening the dialg hen the button is clicked -->
         <v-card-actions>
            <v-spacer></v-spacer>
            <v-btn href="forms"
              color="blue" 
              text @click="dialog = false">ok
            </v-btn>
            <!-- href directs to a certain page -->
            <v-btn href="mediacard"
              color="white" 
              text @click="dialog = false">cancel
            </v-btn>
          </v-card-actions>
        </v-card>
     </v-dialog>

    </v-card-actions>
  </v-card>
</template>