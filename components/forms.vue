<template>
  <v-form v-model="valid">
    <v-container>
      <v-row>
        <h3> Online Debit Card Application </h3>
      </v-row>
      
      <v-layout row justify-center>
         
         <h4> <p class="text-center">CUSTOMER DETAILS </p> </h4>
      </v-layout>

      <v-layout row justify align-content-space-around> 
         
        <v-col cols="6"  md="3">
          <v-text-field ref="form"
            v-model="accountno"
            :rules="accountRules"
            :counter="15"
            label="Account Number"
            filled
          ></v-text-field>
        </v-col>

      </v-layout> 
      <v-row> 
         
        <v-col cols="12" md="3"> 
          <v-text-field ref="form"
            v-model="email"
            :rules="emailRules"
            label="Captcha"
            filled
          ></v-text-field>
        </v-col>
      </v-row>

     <!--<div class="my-2">
        <v-btn flat class="success mx-0 mt-3" @click="submit">OK </v-btn>
      </div>-->

     
      


          <v-card-actions>
            
      <v-dialog v-model="dialog" persistent max-width="390">
      <template v-slot:activator="{ on, attrs }">
        
        <v-btn
          color="primary"
          dark
          v-bind="attrs"
          v-on="on"
        >
             OK  
        </v-btn> 
      </template>
      <v-card>
        <v-btn href="forms"
                icon dark @click="dialog = false">
            <v-icon>mdi-close</v-icon>
        </v-btn>
        <v-card-title class="headline">Successfully Applied For Online Debit Card</v-card-title>
        
        <v-card-actions>
          <v-spacer></v-spacer>
          <v-btn href="mediacard"
          color="blue" 
          text @click="dialog = false">ok</v-btn>
          
        </v-card-actions>
      </v-card>
    </v-dialog>
     
      
    </v-card-actions>
    </v-container>
  </v-form>
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


<script>

  export default {
    data: () => ({
      valid: false,
      accountno: '',
      lastname: '',
      accountRules: [
        v => !!v || 'account number is required',
        v => v.length <= 10 || 'Name must be less than 10 characters',
      ],
      email: '',
      emailRules: [
        v => !!v || 'Captcha is required',
        v => v.length <= 10 || 'Name must be less than 10 characters',
        //v => /.+@.+/.test(v) || 'E-mail must be valid',
      ],
    }),
  }
  //methods: {
  //  submit() {
   //   if(this.$refs.form.validate()){
  //      consol.log(this.title, this.content)
   //   }
 //   }
  //}
    
</script>