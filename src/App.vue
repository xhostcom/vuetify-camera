<template>
<div>
 <v-toolbar
      color="pink"
      dark
    > <v-spacer></v-spacer>
      <v-toolbar-title>Camera</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn icon>
        <v-icon>search</v-icon>
      </v-btn>
    </v-toolbar>
    <v-content>
      <HelloWorld />
    </v-content>
 </div>

</template>

<script>
import HelloWorld from './components/HelloWorld';

export default {
  name: 'App',

  components: {
  HelloWorld,
  },

  data: () => ({
    //
  }),
};
</script>
