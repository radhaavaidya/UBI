<template>
<v-container>

    <v-row
    >
    <v-col
    v-for="i in 3"
    :key=i
    cols="12"
    pa-md="4"
    pa-xs="4"
    pa-lg="4"
    pa-sm="4"
    >
  <v-card
    class="pa-md-4 pa-xs-4 pa-lg-4 pm-md-xs mx-lg-auto"
    
    color="red darken-2"
    width="250px"
  >
    <v-card-text>
      Adjust screen size to see spacing changes
    </v-card-text>
  </v-card>
 </v-col>
    </v-row>
   

  
  </v-container>

</template>