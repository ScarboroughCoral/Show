<template>
  <div class="home">
    <Banner/>
    <v-parallax 
      src="https://cdn.vuetifyjs.com/images/parallax/material.jpg">
    </v-parallax>
    <TreeMenu/>
  </div>
</template>

<script>
// @ is an alias to /src
import Banner from '@/components/Banner.vue'
import TreeMenu from '@/components/TreeMenu.vue';

export default {
  name: 'Home',
  components: {
    Banner,
    TreeMenu
  }
}
</script>
