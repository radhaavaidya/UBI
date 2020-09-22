<template>
<v-container>
    <v-row
    no-gutters
    >
    <v-col md="4" cols4>
       <v-img
       class="mx-auto"
       height="400px"
       src="coker.jpg">
      </v-img>
    </v-col>

     <v-col md="4" cols4>
       <v-img
       class="mx-auto"
       height="400px"
       src="cokest.jpg">
      </v-img>
    </v-col>

    <v-col md="4" cols4>
       <v-img
       class="mx-auto"
       height="400px"
       src="coker.jpg">
      </v-img>
    </v-col>
    </v-row>


  <v-row
    >
    <v-col
    v-for="j in 2"
    :key=j
    cols="6"
    md="6"
    >

      <v-card
        class="red darken-2"
        height="100px"
      >
        <v-card-text>
          <h2> LIFE WITH COKE </h2>
        </v-card-text>
      </v-card>

    </v-col>
  </v-row>
  <v-row >
  <v-col md="6" cols6>
    <span>
    <v-img
      class="text-center grey lighten-2 rounded-circle d-inline-flex align-center justify-center ma-3"
       height="600px"
       src="cokeneechu.jfif">
      </v-img>
    </span>
    </v-col>

    <v-col md="6" cols6>
     <v-card height="600px"> 
      <v-card-text>

          <h1 class="padding"> SOME FACTS ABOUT COKE </h1> <br> <br>
  
          <h4> <li> You cannot enjoy your slice of pizza without a glass full of coke</li> 
               <li> Coca-Cola places sixth in Fortune magazine's annual ranking of the world's 50 most admired companies. </li>
               <li> Coca-Cola has strong brands across its sparkling and still beverages. </li>
               <li> Carbonation makes any drink much more addictive, according to Wenk. </li>
               <li> Coca-Cola has remained the king of carbonated beverages for over 100 years and is doing big things in the world of soda. </li>
               <li> Coca-Cola introduced the first bottles made with recycled material.</li>
               <li> Coca-Cola was the first soft drink in space.</li>
               <li> Coca-Cola still uses the script logo that Frank Robinson crafted in 1891. </li>
               <li> Only a handful of people know the Coca-Cola recipe.</li>
               <li> The “Cola” part of Coca-Cola’s name reportedly comes from the kola nut, a West African nut that is packed with caffeine.</li>
               <li> Mexicans are the largest consumers of Coke annually.</li>
               <li> The drink was first sold as a nerve tonic that “relieves exhaustion.”</li>
               <li> If all the Coca-Cola bottles in the world were laid end to end, they’d reach the moon and back more than 1,677 times.</li>
          </h4>
      </v-card-text>
             
    </v-card> 
    </v-col>
  </v-row>
</v-container>

  </template>
 
  
  