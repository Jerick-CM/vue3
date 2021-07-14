<template>
  <v-app>
    <v-app-bar color="deep-purple" dark>
      <v-btn> <router-link to="/"> <v-icon icon="mdi-home" />Home</router-link> |</v-btn>
      <v-btn> <router-link to="/about">About</router-link></v-btn>
    </v-app-bar>

    <v-main>
      <router-view />
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: "App",

  data: () => ({
    drawer: false,
    group: null,
  }),
};
</script>
