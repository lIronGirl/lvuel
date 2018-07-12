<template>
  <div class="header">
      <div class="header-left">
        <div class="iconfont">&#xe697;</div>
      </div>
      <div class="header-input">
        <span class="iconfont">&#xe6ac;</span>
        输入城市/景点/游玩主题
      </div>
      <div class="header-right">
        城市
        <span class="iconfont">&#xe6aa;</span>
      </div>
  </div>
</template>

<script>
export default {
  name: 'HomeHeader'
}
</script>

<style lang="stylus" scoped>
  @import '~styles/varibles.styl'
  .header
    display: flex
    line-height : .86rem
    background : $bgColor
    color: #fff
    .header-left
      width: .64rem
      float left
      text-align center
      .iconfont
        font-size .6rem
    .header-input
      flex 1
      height .64rem
      line-height .64rem
      margin-top .12rem
      margin-left .2rem
      padding-left .2rem
      background #ffffff
      border-radius .1rem
      color #cccccc
    .header-right
      width 1.24rem
      float right
      text-align center
      .iconfont
        margin-left -.04rem
</style>
