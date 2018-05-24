<template>
<div class="wrapper">
 <swiper :options="swiperOption">
    <swiper-slide>
      <img class="swiper-img" src="http://img1.qunarzz.com/piao/fusion/1804/22/a952a8f7bb956c02.jpg_890x330_5887dc6a.jpg" />
    </swiper-slide>
    <swiper-slide>
      <img class="swiper-img" src="http://img1.qunarzz.com/piao/fusion/1805/f3/91b648c52c4a5a02.jpg_890x330_ea0ef702.jpg" />
    </swiper-slide>
    <div class="swiper-pagination"  slot="pagination"></div>
</swiper>
</div>
</template>
<script>
export default{
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
.wrapper>>> .swiper-pagination-bullet-actieve
  background: #fff
.wrapper
  width: 100%
  height: 0
  overflow: hidden
  padding-bottom: 31.25%
  background: #eee
.swiper-img
  width: 100%
</style>
