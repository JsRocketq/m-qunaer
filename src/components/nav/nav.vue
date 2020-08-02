<template>
    <div class="nav">
       <ul class="nav-list">
         <li
            class="nav-item"
            v-for="item of iconlist" :key="item.id">
           <a href="" class="nav-link">
             <img :src="item.iconUrl" alt="" class="nav-img">
             <span class="nav-text">{{item.iconText}}</span>
           </a>
         </li>
       </ul>
    </div>
</template>

<script>
import item1 from './img/nav-item-1.png'
import item2 from './img/nav-item-2.png'
import item3 from './img/nav-item-3.png'
import item4 from './img/nav-item-4.png'
import item5 from './img/nav-item-5.png'
import item6 from './img/nav-item-6.png'
import item7 from './img/nav-item-7.png'
import item8 from './img/nav-item-8.png'
import item9 from './img/nav-item-9.png'
import item10 from './img/nav-item-10.png'
export default {
  name: 'HomeNav',
  data () {
    return {
      iconlist: [
        {
          id: '01',
          iconUrl: item1,
          iconText: '团购'
        },
        {
          id: '02',
          iconUrl: item2,
          iconText: '购物车'
        }, {
          id: '03',
          iconUrl: item3,
          iconText: '领劵'
        }, {
          id: '04',
          iconUrl: item4,
          iconText: '攻略'
        }, {
          id: '05',
          iconUrl: item5,
          iconText: '机票'
        }, {
          id: '06',
          iconUrl: item6,
          iconText: '美食'
        }, {
          id: '07',
          iconUrl: item7,
          iconText: '饮品'
        }, {
          id: '08',
          iconUrl: item8,
          iconText: '秒杀'
        }, {
          id: '09',
          iconUrl: item9,
          iconText: '抢拍'
        }, {
          id: '10',
          iconUrl: item10,
          iconText: '充值'
        }
      ]
    }
  }
}
</script>

<style lang="stylus" scoped>
  .nav
    width 100%
    padding-top 0.15rem
    background-color #fff
    .nav-list
      display flex
      flex-wrap wrap
      .nav-item
        width 20%
        margin-bottom 0.15rem
        .nav-link
          display flex
          justify-content center
          align-items center
          flex-direction column
          .nav-img
            width 65%
            margin-bottom 0.1rem
</style>
