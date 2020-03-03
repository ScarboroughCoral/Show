<template>
  <div class="home">
    <Banner/>
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
