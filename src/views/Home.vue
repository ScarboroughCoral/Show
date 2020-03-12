<template>
  <div class="home">
    <Banner/>
    <TreeMenu/>
    <v-parallax
      height="1000"
      src="https://file.moetu.org/images/2020/03/12/parallax278dedc1043d0c28.jpg">
    </v-parallax>
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
