<template>
    <div class="icons">
        <swiper :options="swiperOption">
    <!-- slides -->
            <swiper-slide>
                <div class="icon" v-for="icon of iconList" :key="icon.id">
                    <img class="icon-img" :src="icon.imgUrl">
                    <p class="icon-desc">{{ icon.desc }}</p>
                </div>
            </swiper-slide>
        </swiper>
    </div>
</template>

<script>
export default {
  name: 'HomeIcons',
  data() {
    return {
      iconList: [{
        id: '0001',
        imgUrl: 'https://pics.lvjs.com.cn/pics/super/2018/01/1516938549_25686.png',
        desc: '旅行必备'
      }, {
        id: '0002',
        imgUrl: 'https://pics.lvjs.com.cn/pics/super/2017/12/1514474349_75047.png',
        desc: '自驾游'
      }, {
        id: '0003',
        imgUrl: 'https://pics.lvjs.com.cn/pics/super/2018/01/1529646252_29632.png',
        desc: '玩水季'
      }, {
        id: '0004',
        imgUrl: 'https://pics.lvjs.com.cn/pics/super/2018/01/1514474245_92479.png',
        desc: '驴悦亲子游'
      }, {
        id: '0005',
        imgUrl: 'https://pics.lvjs.com.cn/pics/super/2018/01/1525256515_44403.png',
        desc: '国际机票'
      }, {
        id: '0006',
        imgUrl: 'https://pics.lvjs.com.cn/pics/super/2018/01/1530699074_45895.png',
        desc: '特价门票'
      }, {
        id: '0007',
        imgUrl: 'https://pics.lvjs.com.cn/pics/super/2018/01/1523252783_60535.png',
        desc: '签到'
      }, {
        id: '0008',
        imgUrl: 'https://pics.lvjs.com.cn/pics/super/2018/01/1514474202_85264.png',
        desc: '签证'
      }, {
        id: '0009',
        imgUrl: 'https://pics.lvjs.com.cn/pics/super/2018/03/1520416990_47578.png',
        desc: '长隆'
      }, ]
    }
  }
}
</script>

<style lang="stylus" scoped>
  @import '~styles/varibles.styl'
  .icons >>> .swiper-container
    height 0
    padding-bottom 50%
  .icon
    float left
    width 25%
    height 0
    padding-bottom 25%
    text-align center
    .icon-img
      width 70%
    .icon-desc
      margin-top 8%
      color $darkTextColor
</style>
