<template>
  <v-app>
    <v-app-bar
      app
      color="grey lighten-1"
      flat
      inverted-scroll
      dark
    >
      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="@/assets/logo.png"
          transition="scale-transition"
          width="40"
        />

        <h1>二哈妙妙屋</h1>
      </div>

      <v-spacer></v-spacer>

      <v-btn
        href="https://github.com/ScarboroughCoral/Show"
        target="_blank"
        text
      >
        <span class="mr-2">GitHub</span>
        <v-icon>mdi-dog</v-icon>
      </v-btn>
      <!-- <template v-slot:extension>
        <v-tabs align-with-title>
          <v-tab>Tab 1</v-tab>
          <v-tab>Tab 2</v-tab>
          <v-tab>Tab 3</v-tab>
        </v-tabs>
      </template> -->
    </v-app-bar>
    <router-view></router-view>
 
  </v-app>
</template>

<script>

export default {
  name: 'App',

  data: () => ({
    //
  }),
};
</script>
