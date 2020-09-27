<template>
  <div class="text-center">
    <v-menu
      open-on-hover
      top
      offset-y
    >
      <template v-slot:activator="{ on, attrs }">
        <v-btn
          color="primary"
          dark
          v-bind="attrs"
          v-on="on"
          height="48"
          width="20"
        >
          MENU
        </v-btn>
      </template>

      <v-list>
        <v-list-item
          v-for="(item, index) in items"
          :key="index"
        >
          <v-list-item-title>{{ item.title }}</v-list-item-title>
        </v-list-item>
      </v-list>
    </v-menu>
  </div>
  <!-- items are defined in the scripts to make a list  -->
</template>
 


<script>
  export default {
    data: () => ({
      items: [
        { title: 'PRODUCTS' },
        { title: 'DIGITAL BANKING' },
        { title: 'INVESTOR RELATION' },
        { title: 'ABOUT US' },
        { title: 'OTHERS' },
        { title: 'WE CARE' },
      ],
    }),
  }
  // items are the titles in the dropdown of the navigation bar for the smaller screens
</script>
