<template>
  <div>
    <v-breadcrumbs :items="items" divider="-"></v-breadcrumbs>
  </div>
</template>

<script>
  export default {
    data: () => ({
      items: [
        {
          text: 'Home',
          disabled: false,
          href: 'breadcrumbs_dashboard',
        },
        {
          text: 'Cards',
          disabled: false,
          href: 'breadcrumbs_link_1',
        },
        {
          text: 'Debit Cards',
          disabled: false,
          href: 'breadcrumbs_link_2',
        },
        {
          text: 'Classic Debit Card',
          disabled: false,
          href: 'breadcrumbs_link_2',
        },
        {
          text: 'Debit Card Application',
          disabled: false,
          href: 'index',
        },
        
      ],
    }),
  }
  // href direct to the page when clicked on the breadcrumb
</script>