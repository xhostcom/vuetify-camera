<template>
  <v-container>
          <v-img
          alt="iTunes Logo"
          class="shrink"
          contain
          src="../assets/appled.webp"
          transition="scale-transition"
          width="80"
        />
     <v-card
    class="d-flex pa-2 justify-content-center"
    outlined
    tile
  >
    <div> <h1>Hello</h1>
</div>
  </v-card>


  </v-container>


</template>
<script>
  export default {
    name: 'HelloWorld',

    data: () => ({
      ecosystem: [
        {
          text: 'vuetify-loader',
          href: 'https://github.com/vuetifyjs/vuetify-loader',
        },
        {
          text: 'github',
          href: 'https://github.com/vuetifyjs/vuetify',
        },
        {
          text: 'awesome-vuetify',
          href: 'https://github.com/vuetifyjs/awesome-vuetify',
        },
      ],
      importantLinks: [
        {
          text: 'Documentation',
          href: 'https://vuetifyjs.com',
        },
        {
          text: 'Chat',
          href: 'https://community.vuetifyjs.com',
        },
        {
          text: 'Made with Vuetify',
          href: 'https://madewithvuejs.com/vuetify',
        },
        {
          text: 'Twitter',
          href: 'https://twitter.com/vuetifyjs',
        },
        {
          text: 'Articles',
          href: 'https://medium.com/vuetify',
        },
      ],
      whatsNext: [
        {
          text: 'Explore components',
          href: 'https://vuetifyjs.com/components/api-explorer',
        },
        {
          text: 'Select a layout',
          href: 'https://vuetifyjs.com/layout/pre-defined',
        },
        {
          text: 'Frequently Asked Questions',
          href: 'https://vuetifyjs.com/getting-started/frequently-asked-questions',
        },
      ],
    }),
  }
</script>
<script>
export default {
    name: 'camera'
}
</script>

<style scoped>
.camera {
    width: 100%;
    height: 100vh;
    padding: 25px;
    box-sizing: border-box;
}
.feed {
    width: 100%;
    max-width: 1280px;
    margin: 0 auto;
    background-color: #171717;
    box-shadow: 6px 6px 12px 0px rgba(0,0,0,0.25);
}
</style>
