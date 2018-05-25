<template>
<div class="wrapper">
 <swiper :options="swiperOption">
    <swiper-slide>
      <img class="swiper-img" src="http://img1.qunarzz.com/piao/fusion/1805/77/f63bd04dd5319602.jpg_750x200_6ba8e0ca.jpg" />
    </swiper-slide>
    <swiper-slide>
      <img class="swiper-img" src="http://img1.qunarzz.com/piao/fusion/1805/82/62ed2855921b1302.jpg_750x200_cb7e0793.jpg" />
    </swiper-slide>
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
        pagination: '.swiper-pagination'
      }
    }
  }
}
</script>
<style lang="stylus" scoped>
  .wrapper >>> .swiper-pagination-bullet-active
    background: #fff
  .wrapper
    overflow: hidden
    width: 100%
    height: 0
    padding-bottom: 31.25%
    background: #eee
  .swiper-img
    width: 100%
</style>
