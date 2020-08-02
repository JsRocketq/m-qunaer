<template>
  <div class="wrapper">
    <swiper :options="swiperOption">
      <!-- slides -->
      <swiper-slide v-for="item in swiperlist" :key="item.id">
        <img class="swiper-img" :src="item.imgUrl" alt="">
      </swiper-slide>
      <!-- Optional controls -->
      <div class="swiper-pagination"  slot="pagination"></div>
    </swiper>
  </div>
</template>

<script>
import one from './img/1.jpg'
import two from './img/2.jpg'
import three from './img/3.jpg'
import four from './img/4.jpg'

export default {
  name: 'HomeSwiper',
  data () {
    return {
      swiperOption: {
        pagination: {
          el: '.swiper-pagination'
        },
        loop: true,
        autoplay: true,
        speed: 1000
      },
      swiperlist: [{
        id: '01',
        imgUrl: one
      }, {
        id: '02',
        imgUrl: two
      }, {
        id: '03',
        imgUrl: three
      }, {
        id: '04',
        imgUrl: four
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
  .wrapper >>> .swiper-pagination-bullet-active
    background #fff
  .wrapper
    width 100%
    height 175px
    overflow hidden
    .swiper-img
      width 100%
</style>
