<template>

  <v-card
    class="mx-auto"
    max-width="400">
    
    <v-img
      class="mx-auto"
      height="300px"
      src="icons-02.jpg">
    </v-img>

    <v-card-text 
      class="text--primary">
    </v-card-text>

    <v-card-actions>
      <v-dialog v-model="dialog" persistent max-width="420">
        <template v-slot:activator="{ on, attrs }">
          <v-btn
            color="primary"
            dark
            v-bind="attrs"
            v-on="on" >
            Online Debit Card Tracking
          </v-btn> 
        </template>
      </v-dialog>
    </v-card-actions>
  </v-card>
</template>