<template>
 <swiper :options="swiperOption">
    <swiper-slide>
      <img src="http://img1.qunarzz.com/piao/fusion/1804/22/a952a8f7bb956c02.jpg_890x330_5887dc6a.jpg"/>
    </swiper-slide>
    <swiper-slide>
      <img src="http://img1.qunarzz.com/piao/fusion/1804/97/097b9aa3b6815302.jpg_890x330_a74265fc.jpg"/>
    </swiper-slide>
    <div class="swiper-pagination"  slot="pagination"></div>
</swiper>
</template>
<script>
export default{
  name: 'HomeSwiper',
  data () {
    return {
      swiperOption: {}
    }
  }
}
</script>
<style lang="stylus" scoped>

</style>
