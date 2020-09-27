<template>
  <!--Your App Starts Here -->
  <v-app id="inspire">
    
    <!--Header -->
    <v-app-bar color="#E22026" dark fixed app>
      <!-- <v-toolbar-title>Application</v-toolbar-title> -->
       <!-- Component Example -->

      <logoubi/> 
      <v-col> </v-col>
      <v-row class="hidden-sm-and-down">
         <navbaring/> 
      </v-row> 
      <v-row class="hidden-md-and-up">
        <v-col sm="9"></v-col>
        <v-col sm="1" class="mb-sm-2 ma-sm-2 mb-2 ma-2 mx-0" >
 <!-- the class helps in defining the placement and sizing of the menu button in different screen sizes -->
 <!-- class hidden helps in hiding the navigation bar under those conditions -->
         <navchotu/>
        </v-col>
      </v-row>
      
  
      <!-- the universal navigation bar -->
      
    </v-app-bar>

    <!-- Body -->
    
    <v-content light>

      <bread/>
      <!-- breadcrumb -->

      <nuxt /> 
      
    </v-content>

     <!--footer  -->

    <v-footer color="#DA2627">
      <v-img
       class="mx-auto"
       src="footer.png" >
      </v-img>
    </v-footer>
      
  </v-app>
</template>

<script>
export default {}
</script>

<style> 
  .white--text {
    border: 1px solid;
  }

   #inspire {
    background-color: white;
    color: rgb(255, 255, 255);
  }
</style>