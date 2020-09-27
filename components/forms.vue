<template>
  <v-form v-model="isFormValid">
             <!--enabeling and disableing the submit button(validating) -->
    <v-container>
    
      <v-row>
         <h3 class="hey"> Online Debit Card Application </h3>
         
      </v-row>
      
             <!-- h3 and h4- sizes of the text -->
      <br>
      <v-layout row justify-center class="hey">
         <h4> <p class="text-center">CUSTOMER DETAILS </p> </h4>
      </v-layout>

      <v-row justify="center"> 
        <v-col cols="7" md="7" sm="7">
          <v-text-field ref="form"
            dark="false"
            v-model="accountno"
            type="password"
            :rules="accountRules"
            :counter="15"
            label="Account Number*"
            filled>
          </v-text-field> 
        </v-col>
      </v-row> 
             <!-- type password converts the content into bullets -->
             <!-- rules field according to the script enebles the reqired and the no. of characters required-->
             <!-- counter shows number of characters alloweed -->

      <v-row justify="center"> 
        <v-col cols="7" md="7" sm="7">
          <v-text-field ref="form"
           v-model="reaccountno"
            type="password"
            :rules="reaccountRules"
            :counter="15"
            label="Re-enter account Number*"
            filled >
          </v-text-field> 
        </v-col>
     </v-row> 

     <v-row justify="center">
        <v-col cols="7" md="7" sm="7"> 
          <v-text-field ref="form"
            v-model="email"
            :rules="emailRules"
            label="Captcha*"
            filled >
          </v-text-field>
        </v-col>
     </v-row>
      <!-- sm md helps in defining the grids in a perticular screen type like sm is for ipads xs is for all the phones md i the laptop screen,etc -->
     <v-row justify="center">
        <v-col cols="3" md="4" sm="4">
          <v-img
           class="mx-auto"
           max-height="100px"
           max-width="220px"
           src="captcha.png">
          </v-img>
        </v-col>
      </v-row> 

      <v-row justify="center" >
         <em text id="require">*Required</em>
      </v-row>
            <!-- Justify center aligns it to the centre -->
            <!-- em text makes the text italic -->

      <v-card-actions>
        <v-dialog v-model="dialog" persistent max-width="390">
           <template v-slot:activator="{ on, attrs }">
             <v-row justify="center">
               <v-col cols="1">  
                 <v-btn 
                   :disabled="!isFormValid"
                   color="primary"
                   dark
                   v-bind="attrs"
                   v-on="on">
                   OK  
                 </v-btn> 
               </v-col>
             </v-row>
           </template>
            <!-- href directs form one page to another -->
            <!-- :disabled ensures that the button is disabled till the form is filled -->
          <v-card>
            <v-btn href="forms" 

              icon dark @click="dialog = false">
                <v-icon>
                  mdi-close
                </v-icon>
            </v-btn>

              <v-card-title class="headline">
                Successfully Applied For Online Debit Card
              </v-card-title>
        
              <v-card-actions>
                <v-spacer></v-spacer>

                <v-btn href="mediacard"
                  color="blue" 
                  text @click="dialog = false">
                  ok
                </v-btn>
              </v-card-actions>
          </v-card>
       </v-dialog>
      </v-card-actions>

    </v-container>
  </v-form>
</template>

<style> 
  .hey {
    color: rgb(47, 64, 143);
    font-family: Arial;
  }
  /* .hey is used to make a class and #is used to create a unique set */

  .black--text {
    border: 1px solid;
  }

   #inspire {
    background-color: rgb(196, 193, 193);
    color: rgb(255, 255, 255);
  }
  
  #require {
    color: red;
    font-family: Arial;
  }

</style>

<script>

  export default {
    data: () => ({
      isFormValid: false,
      accountno: '',
      reaccountno: '',
      lastname: '',
      accountRules: [
        v => !!v || 'account number is required',
        v => v.length <= 15 || 'Name must be less than 15 characters',
      ],
      // ensures that the textfield is filled under the above conditions
      reaccountRules: [
        v => !!v || 're entering the account number is required',
        v => v.length <= 15 || 'Name must be less than 15 characters',
      ],

      email: '',
      emailRules: [
        v => !!v || 'Captcha is required',
      ],
    }),
  }
</script>