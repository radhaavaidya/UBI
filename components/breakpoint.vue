<template>
  <v-container>

    <v-row
    >
    <v-col
    v-for="i in 3"
    :key=i
    cols="12"
    md="4"
    sx="4"
    lg="4"
    >
    
      <v-card
        class="ma-3 pa-3 mx-lg-auto"
      >
        <v-card-text>
          3 cards
        </v-card-text>
      </v-card>

    </v-col>
    </v-row>
   

  
  </v-container>  
</template>


<style> 
  .black--text {
    border: 1px solid;
  }

   #inspire {
    background-color: rgb(196, 193, 193);
    color: rgb(255, 255, 255);
  }
</style>