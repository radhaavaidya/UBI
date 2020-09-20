<template>
  <!--Your App Starts Here -->
  <v-app id="inspire">
    
    <!--Header -->
    
    <v-app-bar 
      color="#E22026">
      <navbar/>

      <tab/>
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