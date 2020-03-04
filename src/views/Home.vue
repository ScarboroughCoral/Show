<template>
  <div class="home">
    <Banner/>
    <v-parallax
      height="1000"
      src="@/assets/parallax.jpg">
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
