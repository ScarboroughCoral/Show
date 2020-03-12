<template>
  <v-app>
    <v-app-bar
      app
      color="grey lighten-1"
      inverted-scroll
      dark
    >
      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="https://file.moetu.org/images/2020/03/12/logof20aa56253a79f08.png"
          transition="scale-transition"
          width="40"
        />

        <h1 class="d-none d-sm-flex">二哈妙妙屋</h1>
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

<script lang="ts">

export default {
  name: 'App',

  data: () => ({
    //
  }),
};
</script>
