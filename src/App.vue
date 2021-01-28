<template>
  <v-app>
    <v-navigation-drawer 
    v-model="nav"
    app
    absolute
    temporary
    >

    </v-navigation-drawer>

      <!-- v-btn v-on: click="nav =!nav">Button</v-btn> -->

    <v-content class="px-12 py-3" app>
      <v-container fluid>
        <router-view/>
      </v-container>
    </v-content>

  </v-app>
</template>

<script>

export default {
  name: 'App',

  components: {
  },

  data: () => ({
    nav: false
  }),
};
</script>
