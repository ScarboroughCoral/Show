<template>
  <v-carousel
    cycle
    height="100vh"
    show-arrows-on-hover
  >
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
    >
      <v-sheet
        height="100vh"
        color="transparent"
      >
        <v-row
          class="fill-height"
          align="center"
          justify="center"
        >
          <div class="display-2 pa-5">{{ item.desc||"" }}</div>
        </v-row>
      </v-sheet>
    </v-carousel-item>
  </v-carousel>
</template>

<script>
import Dou from '@/assets/slides/dou.jpg';
import ZongHeng from '@/assets/slides/genie.jpg';
import MingZuo from '@/assets/slides/mingzuo.jpg';
  export default {
    data () {
      return {
        items: [
          {
            src: Dou,
            desc:'纵使我身形俱灭，也定将恶鬼斩杀',
            color:"green--text text--light-2"
          },
          {
            src: 'http://119.36.226.152/update1.dlied.qq.com/dnf/website/wallpaper/wallpaper_201508.jpg?mkey=5e5f07c17b8670c9&f=d510&cip=123.134.86.60&proto=http&access_type=$header_ApolloNet',
            desc:'用耳去听，用心去看。——G.S.D',
          },
          {
            src: ZongHeng,
            desc:'怒而诸侯俱，安居而天下熄。——唯我纵横'
          },
          {
            src: MingZuo,
            desc: '你毁了我世界的唯一，我便毁了你们唯一的世界。'
          },
        ],
      }
    },
  }
</script>
<style scoped>

</style>