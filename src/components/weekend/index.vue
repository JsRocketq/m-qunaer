<template>
    <div>
        <div class="weekend-title">周末去哪儿</div>
        <ul class="weekend-wrapper" v-for="item of weekendList" :key='item.key'>
            <li class="weekend-item">
                <div class="img-wraper">
                    <img :src="item.imgUrl" alt="">
                </div>
                <div class="text-wrapper">
                    <p class="weekend-text">金奖提名佳作</p>
                    <p class="weekend-desc">三俩好友，吃喝玩乐，尊享优质电影</p>
                </div>
            </li>
        </ul>
    </div>
</template>

<script>
import one from './img/bl.png'
import two from './img/cat.png'
import three from './img/crab.png'
import four from './img/sls.jpg'
import five from './img/vr.png'
import six from './img/xiaolong.jpg'
export default {
  name: 'HomeWeekend',
  data () {
    return {
      weekendList: [
        {
          id: 1,
          imgUrl: one,
          text: '金奖提名佳作',
          desc: '三俩好友，吃喝玩乐，尊享优质电影'
        },
        {
          id: 2,
          imgUrl: two,
          text: '金奖提名佳作',
          desc: '三俩好友，吃喝玩乐，尊享优质电影'
        },
        {
          id: 3,
          imgUrl: three,
          text: '金奖提名佳作',
          desc: '三俩好友，吃喝玩乐，尊享优质电影'
        },
        {
          id: 4,
          imgUrl: four,
          text: '金奖提名佳作',
          desc: '三俩好友，吃喝玩乐，尊享优质电影'
        },
        {
          id: 5,
          imgUrl: five,
          text: '金奖提名佳作',
          desc: '三俩好友，吃喝玩乐，尊享优质电影'
        },
        {
          id: 6,
          imgUrl: six,
          text: '金奖提名佳作',
          desc: '三俩好友，吃喝玩乐，尊享优质电影'
        }
      ]
    }
  }
}
</script>

<style lang="stylus">
    .weekend-title
        background-color #eee
        text-indent .2rem
        font-weight bold
    .img-wraper
        margin-top .18rem
        overflow: hidden
        width 100%
        height 2.5rem
    .text-wrapper
        padding .18rem
        .weekend-text
            font-weight bold
            font-size .35rem
            line-height .35rem
            height .35rem
        .weekend-desc
            color #888
            margin-top .18rem
            line-height .2rem
</style>
