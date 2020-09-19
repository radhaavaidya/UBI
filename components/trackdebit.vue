<template>

  <v-card
    class="mx-auto"
    max-width="400"
  >
    <v-img
      class="mx-auto"
      height="300px"
      src="icons-02.jpg"
    >
     <!-- <v-card-title>Top 10 Australian beaches</v-card-title>-->
    </v-img>

    <!--<v-card-subtitle class="pb-0">Number 10</v-card-subtitle>-->
    <!--v-card-title> Apply for Online Debit Card</v-card-title>-->
    <v-card-text class="text--primary">
      <!--<div>Whitehaven Beach</div>

      <div>Whitsunday Island, Whitsunday Islands</div>-->
    </v-card-text>

    <v-card-actions>
      <v-dialog v-model="dialog" persistent max-width="290">
      <template v-slot:activator="{ on, attrs }">
        <v-btn
          color="primary"
        >
          Online Application Tracking
        </v-btn> 
      </template>
      
    </v-dialog>

      <!--<v-btn
        color="orange"
        text
      >
        Explore
      </v-btn>-->
    </v-card-actions>
  </v-card>
</template>