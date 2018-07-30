<template>
<div class="recommend">
  <div class="recommend-title">热销推荐</div>
  <ul class="recommend-list">
    <li class="recommend-item">
      <img src="http://img1.qunarzz.com/sight/p0/1803/12/126471e0966aca5ba3.img.jpg_200x200_f1286016.jpg" alt="北京国际鲜花港">
      <p class="recommend-item-title">北京国际鲜花港</p>
      <div>
        <span class="recommend-item-rate iconfont">&#58886;</span>
        <span class="recommend-item-comment-count">1927条评论</span>
      </div>
      <div>
        <span class="recommend-item-price"><span>￥19.9</span>起</span><span class="recommend-item-local">顺义区</span>
      </div>
    </li>
  </ul>
</div>
</template>

<script>
export default {
  name: 'HomeRecommend'
}
</script>

<style lang="stylus" scoped>
.recommend-title
  background-color #eee
  line-height .8rem
  text-indent .2rem
.recommend-list
  margin-left .24rem
  .recommend-item
    padding .2rem 0
    img
      float left
      margin-right .26rem
      width 2rem
      height 2rem
    .recommend-item-title
      margin-top .26rem
      font-size .32rem
    div
      .iconfont
        font-size .6rem
</style>
