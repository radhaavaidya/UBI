<template>
  <v-tabs
   
    background-color="#E22026"
    
    <v-tabs color="red darken-4"
    dark 
    >
    <logoubi/>
    <v-tab>
      PRODUCTS
    </v-tab>
    <v-tab>
      DIGITAL BANKING
    </v-tab>
    <v-tab>
      INVESTOR RELATION
    </v-tab>
    <v-tab>
     ABOUT US
    </v-tab>
    <v-tab>
      OTHERS
    </v-tab>
    <v-tab>
      WE CARE
    </v-tab>

    <v-spacer></v-spacer>

     <v-btn icon class="hidden-xs-only">
       <v-icon>mdi-magnify</v-icon>
     </v-btn>
<!-- search -->
     
     <v-col  cols="2" >
      <v-text-field
            label="SEARCH"
            outlined 
      ></v-text-field>
    </v-col>
<!-- Adds text field for the search -->
<!-- cols define the space taken -->
<!-- v-spacer creates the space between the seach icon and the rest of the tabs -->
    
</v-tabs>
</template>
