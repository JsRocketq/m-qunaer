<template>
    <div>
        <home-header></home-header>
        <home-swiper></home-swiper>
        <home-nav></home-nav>
        <home-recommend></home-recommend>
        <home-weekend></home-weekend>
    </div>
</template>

<script>
import HomeHeader from '../../components/header/header'
import HomeSwiper from '../../components/swiper/swiper'
import HomeNav from '../../components/nav/nav'
import HomeRecommend from '../../components/recommend/recommend'
import HomeWeekend from '../../components/weekend/index'
import axios from 'axios'
export default {
  name: 'Home',
  components: {
    HomeHeader,
    HomeSwiper,
    HomeNav,
    HomeRecommend,
    HomeWeekend
  },
  methods: {
    getHomeInfo () {
      axios.get('/api/index.json')
        .then(this.getHomeInfoSucc)
    },
    getHomeInfoSucc (res) {
      console.log(res)
    }
  },
  mounted () {
    this.getHomeInfo()
  }
}
</script>

<style lang="stylus">
</style>
