<template>
  <v-responsive class="pa-2 purple lighten-5" >
    <v-lazy
      v-model="isActive"
      :options="{
          threshold: .5
        }"
      min-height="200"
      :transition="i%2?'slide-x-reverse-transition':'slide-x-transition'"
       v-for="(item,i) in items" :key="i"
    >
    <v-card
    class="mx-auto ma-12"
    elevation="6"
    max-width="400"
  >
    <v-img
      class="white--text align-end"
      height="200px"
      :src="item.img||'https://cdn.vuetifyjs.com/images/cards/docks.jpg'"
    >
      <v-card-title>{{item.title}}</v-card-title>
    </v-img>
    <v-card-text class="text--primary">
      {{item.desc}}
    </v-card-text>
    <v-card-actions>
      <v-btn
        color="orange"
        text
        :href="item.path"
      >
        Explore
      </v-btn>
    </v-card-actions>
  </v-card>
    </v-lazy>
  </v-responsive>
</template>

<script lang="ts">
import items from '@/config/menu.ts';

export default {
  data: () => ({
    isActive: false,
    items,
  })
};
</script>

<style scoped>
</style>