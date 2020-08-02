<template>
  <div>
      <div class="recommend-title">热销推荐</div>
      <ul>
        <li class="item border-bottom" v-for="item of listitem" :key="item.id">
            <img class="item-img" :src="item.imgUrl" alt="">
          <div class="item-content">
            <p class="item-title">{{item.title}}</p>
            <p class="item-desc">{{item.desc}}</p>
            <p class="item-price">{{item.price}} <span>起</span></p>
          </div>
        </li>
      </ul>
      <div class="recommend-bottom">
        <p class="bottom-text">查看所有产品</p>
      </div>
  </div>
</template>

<script>
import one from './img/3.jpg'
export default {
  name: 'Recommend',
  data () {
    return {
      listitem: [
        {
          id: 1,
          imgUrl: one,
          title: '宇宙最强最美景点',
          desc: '浪漫的世界，需要你我共同努力，学到了没有',
          price: '￥999'
        },
        {
          id: 2,
          imgUrl: one,
          title: '宇宙最强最美景点',
          desc: '浪漫的世界，需要你我共同努力，学到了没有',
          price: '￥999'
        },
        {
          id: 3,
          imgUrl: one,
          title: '宇宙最强最美景点',
          desc: '浪漫的世界，需要你我共同努力，学到了没有',
          price: '￥999'
        },
        {
          id: 4,
          imgUrl: one,
          title: '宇宙最强最美景点',
          desc: '浪漫的世界，需要你我共同努力，学到了没有',
          price: '￥999'
        },
        {
          id: 5,
          imgUrl: one,
          title: '宇宙最强最美景点',
          desc: '浪漫的世界，需要你我共同努力，学到了没有',
          price: '￥999'
        }
      ]
    }
  }
}
</script>

<style lang="stylus">
  .recommend-bottom
    height .5rem
    line-height .5rem
    .bottom-text
      color rgb(11,182,255)
      text-align center
      font-size .3rem
      font-weight 700
  .recommend-title
    line-height .6rem
    background #eee
    text-indent .3rem
    height .6rem
  .item
    display flex
    height 1.9rem
    overflow hidden
    .item-img
      width 1.7rem
      height 1.7rem
      padding .1rem
    .item-content
      padding .1rem
      flex 1
      min-width 0
      margin-left .1rem
      .item-title
        font-weight 700
        font-size .35rem
        margin-top .2rem
        line-height .35rem
        overflow hidden
        white-space nowrap
        text-overflow ellipsis
      .item-desc
        margin-top .2rem
        color #888
        overflow hidden
        white-space nowrap
        text-overflow ellipsis
      .item-price
        font-size .3rem
        color #ff9300
        padding-top .2rem
        span
          color #888
          font-size .2rem
</style>>
