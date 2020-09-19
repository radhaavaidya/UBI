<template>
  <v-card
    class="string"
    max-width="344"
  >
  <!--the class-function helps in defining the position of card-->
    <v-img
      src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
      height="200px"
    ></v-img>

    <v-card-title>
      Top western road trips
    </v-card-title>

    <v-card-subtitle>
      1,000 miles of wonder
    </v-card-subtitle>

    <v-card-actions>
      <v-btn text>Share</v-btn>

      <v-btn
        color="purple"
        text
      >
        Explore
      </v-btn>

      <v-spacer></v-spacer>
      <!--line 30th the spacer defines the space between the elements-->
        

      <v-btn
        icon
        @click="show = !show"   
      >
      <!--enables the animation of pressing the arrow and the drowdown appearing-->
      
        <v-icon>{{ show ? 'mdi-chevron-down' : 'mdi-chevron-up' }}</v-icon>
        <!--the orentation of the arrow when clicked on it-->
      </v-btn>
    </v-card-actions>

    <v-expand-transition>
      <div v-show="show">
        <!--"hide"- hides the drowdown animation-->
        <v-divider></v-divider>
        <!--adds a thin line bettwen the buttons and the text in the dropdown-->

        <v-card-text>
          I'm a thing. But, like most politicians, he promised more than he could deliver. You won't have time for sleeping, soldier, not with all the bed making you'll be doing. Then we'll go with that data file! Hey, you add a one and two zeros to that or we walk! You're going to do his laundry? I've got to find a way to escape.
        </v-card-text>
      </div>
    </v-expand-transition>
  </v-card>
  
</template>

<script>
  export default {
    data: () => ({
      show: false,
    }),
    //defines the default structure of the card when the page is opened
  }
</script>
 