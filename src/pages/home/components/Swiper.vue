<template>
  <div class="wrapper">
    <swiper :options="swiperOption" ref="mySwiper" @someSwiperEvent="callback">
    <!-- slides -->
    <swiper-slide v-for="swiper of swiperList" :key="swiper.id">
      <img :src="swiper.imgurl" alt="" class="swiper-img">
    </swiper-slide>
    <!-- Optional controls -->
    <div class="swiper-pagination"  slot="pagination"></div>
    </swiper>
  </div>
</template>

<script>
export default {
  name: 'HomeSwiper',
  data () {
    return {
      swiperOption: {
        autoplay: 2000,
        pagination: '.swiper-pagination',
        loop: true
      },
      swiperList: [{
        id: '0001',
        imgurl: 'https://source.qunarzz.com/site/images/wap/home/recommend/iphoneplus/dujia_shuqi_banner_20180710.jpg'
      }, {
        id: '0002',
        imgurl: 'https://source.qunarzz.com/site/images/wap/home/recommend/iphoneplus/20180713_CPM_11053.jpg'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
.wrapper >>> .swiper-pagination-bullet-active
    background #fff
.wrapper
  overflow hidden
  width 100%
  height 0
  padding-bottom 31.25%
  .swiper-img
    width 100%
</style>
