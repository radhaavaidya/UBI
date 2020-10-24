<template>
  <div>
    <v-breadcrumbs
      :items="items"
      large
    ></v-breadcrumbs>
  </div>
</template>
<script>
  export default {
    data: () => ({
      items: [
        {
          text: 'Home',
          disabled: true,
          href: 'breadcrumbs_dashboard',
        },
        {
          text: 'Cards',
          disabled: true,
          href: 'breadcrumbs_link_1',
        },
        {
          text: 'Debit Cards',
          disabled: true,
          href: 'breadcrumbs_link_2',
        },
        {
          text: 'Classic Debit Card',
          disabled: true,
          href: 'breadcrumbs_link_2',
        },
        {
          text: 'Debit Card Application',
          disabled: false,
          href: 'breadcrumbs_link_2',
        },
      ],
    }),
  }
</script>