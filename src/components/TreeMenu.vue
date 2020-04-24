<template>
  <v-responsive class="pa-2 purple lighten-5">
    <v-lazy
      v-model="isActive"
      :options="{
          threshold: .5
        }"
      min-height="200"
      v-for="(item,i) in items"
      :key="i"
    >
      <transition name="slide">
        <v-card class="mx-auto ma-12" elevation="6" max-width="400">
          <v-img
            class="white--text align-end"
            height="200px"
            :src="item.img||'https://cdn.vuetifyjs.com/images/cards/docks.jpg'"
          >
            <v-card-title>{{item.title}}</v-card-title>
          </v-img>
          <v-card-text class="text--primary">{{item.desc}}</v-card-text>
          <v-card-actions>
            <v-btn color="orange" text :href="item.path">Explore</v-btn>
          </v-card-actions>
        </v-card>
      </transition>
    </v-lazy>
  </v-responsive>
</template>

<script lang="ts">
import items from "@/config/menu.ts";

export default {
  data: () => ({
    isActive: false,
    items
  })
};
</script>

<style scoped>
.slide-enter-active {
  transition: 1s;
}
.slide-enter {
  transform: translateX(-200%);
}
</style>