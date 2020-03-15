<template>
<v-app>
    <v-app-bar
      app
      color="dark"
      dark
    >
    <v-icon>mdi-menu</v-icon>
    <v-spacer></v-spacer>
    <v-toolbar-title class="white--text">
      <router-link class="title" to="/">Camera</router-link>
    </v-toolbar-title>
    <v-spacer></v-spacer>
    <v-btn to="/">
    <v-icon>mdi-refresh</v-icon>
    </v-btn>
    </v-app-bar>
    <v-content>
     <Camera />
    </v-content>
  </v-app>
</template>

<script>
import Camera from './components/Camera';

export default {
  name: 'App',

  components: {
  Camera,
  },

  data: () => ({
    //
  }),
};
</script>
