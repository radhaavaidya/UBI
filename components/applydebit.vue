<template>

  <v-card
    class="mx-auto"
    max-width="400"
  >
    <v-img
      class="mx-auto"
      height="300px"
      src="icons-01.jpg"
    >
     
    </v-img>

    <!--<v-card-subtitle class="pb-0">Number 10</v-card-subtitle>-->
    <!--v-card-title> Apply for Online Debit Card</v-card-title>-->
    <v-card-text class="text--primary">
      <!--<div>Whitehaven Beach</div>

      <div>Whitsunday Island, Whitsunday Islands</div>-->
    </v-card-text>

    <v-card-actions>
      <v-dialog v-model="dialog" persistent max-width="420">
      <template v-slot:activator="{ on, attrs }">
        <v-btn
          color="primary"
          dark
          v-bind="attrs"
          v-on="on"
        >
          Apply for online debit card
        </v-btn> 
      </template>
      <v-card>
        <v-card-title class="headline">If you already have an active debit card, Please do not apply for debit card online</v-card-title>
        <!--<v-card-text>If you already have an active debit card, Please do not apply for debit card online</v-card-text>-->
        <v-card-actions>
          <v-spacer></v-spacer>
          <v-btn href="forms"
          color="blue" 
          text @click="dialog = false">ok</v-btn>
          <v-btn href="mediacard"
          color="white" 
          text @click="dialog = false">cancel</v-btn>
        </v-card-actions>
      </v-card>
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