<template>
  <swiper :options="swiperOption" class="swiper-box" ref="mySwiper">
    <!-- slides -->
    <swiper-slide v-for="slide in swiperSlides" :key="slide.id"><img width="100%" height="100%" :src="slide.src" alt=""></swiper-slide>
    <!-- Optional controls -->
    <div class="swiper-pagination"  slot="pagination"></div>
    <div class="swiper-button-prev" slot="button-prev"></div>
    <div class="swiper-button-next" slot="button-next"></div>
    <div class="swiper-scrollbar"   slot="scrollbar"></div>
  </swiper>
</template>

<script>
import 'swiper/dist/css/swiper.css'

import { swiper, swiperSlide } from 'vue-awesome-swiper'
export default {
  name: 'carrousel',
  components: {
    swiper,
    swiperSlide
  },
  data () {
    return {
      swiperOption: {
        pagination: {
          el: '.swiper-pagination'
        },
        autoplay: true
      },
      swiperSlides: [{ src: '/static/1.jpg', id: 1 }, { src: '/static/2.jpg', id: 2 }]
    }
  },
  computed: {
    swiper () {
      return this.$refs.mySwiper.swiper
    }
  },
  mounted () {
  //   console.log('this is current swiper instance object', this.swiper)
  //   this.swiper.slideTo(1, 1000, false)
  //   this.swiper.startAutoplay()
  }
}
</script>
<style lang="stylus" scoped>
.swiper-box
  width 625px
  height 273px
  img
    width 100%
    height 100%
</style>
