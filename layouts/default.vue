<template>
  <!--Your App Starts Here -->
  <v-app id="inspire">
    
    <!--Header -->
    <UBIlogo/>
    
    <v-app-bar color="#E22026"  >
      <v-btn color="#E22026" depressed small >
        PRODUCTS
      </v-btn>
      
      <v-btn color="#E22026" depressed small >
       DIGITAL BANKING
      </v-btn>

      <v-btn color="#E22026" depressed small >
        INVESTOR RELATIONS
      </v-btn>

      <v-btn color="#E22026" depressed small >
        ABOUT US
      </v-btn>

      <v-btn color="#E22026" depressed small >
        OTHERS
      </v-btn>

      <v-btn color="#E22026" depressed small >
        WE CARE
      </v-btn>
      

      <!-- <v-toolbar-title>Application</v-toolbar-title> -->
       <!-- Component Example -->
      <Ubilogo/> <tab/>
    </v-app-bar>

    <!-- Body -->
    
    <v-content light>
      <nuxt /> <v-img
      class="mx-auto"
      
      src="footer.png"
    >
     
    </v-img>
    </v-content>
    
    <!-- Footer 

    <v-footer color="#E22026" app>
      <span class="white--text">&copy; 
        
              
        {{ new Date().getFullYear() }}</span>
    </v-footer>-->

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