<template>
    <div class="header">
        <div class="header-left">
            <div class="iconfont back-icon">&#xe624;</div>
        </div>
        <div class="header-center">
            <span class="iconfont">&#xe632;</span>
            输入城市/景点/游玩主题
            </div>
        <div class="header-right">
            城市
            <span></span>
        </div>
    </div>
</template>

<script>
export default {
  name: 'HomeHeader'
}
</script>
<style lang="stylus" scoped>
     .header
        background-color #00bcd4
        display flex
        height .86rem
        line-height .86rem
        color #fff
        .header-left
            width .64rem
            float left
            .back-icon
                text-align center
                font-size .4rem
        .header-center
            flex 1
            background-color #fff
            border-radius .1rem
            margin-top .12rem
            height .64rem
            margin-left .2rem
            color #ccc
            line-height .64rem
            padding-left .2rem
            .search
                line-height .64rem
        .header-right
            width 1.24rem
            float right
            text-align center
            span
                display inline-block
                position relative
                top .1rem
                width 0
                height 0
                border .14rem solid transparent
                border-top-color #fff
                margin-left .02rem
</style>
