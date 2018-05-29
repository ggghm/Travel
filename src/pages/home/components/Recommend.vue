<template>
  <div>
    <div class="title">猜你喜欢</div>
    <ul>
      <li class="item border-bottom" v-for="item of recommendList" :key="item.id">
        <img class="item-img" :src="item.imgUrl" />
        <div class="item-info">
          <p class="item-title">{{item.title}}</p>
          <p class="item-desc">{{item.desc}}</p>
          <button class="item-button">查看详情</button>
        </div>
      </li>
    </ul>
  </div>
</template>
<script>
export default {
  name: 'HomeWeekend',
  data () {
    return {
      recommendList: [{
        id: '0001',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1705/ed/edd4063a442f30c1a3.img.jpg_200x200_724f9e6a.jpg',
        title: '北京欢乐谷',
        desc: '近期小伙伴们收藏最！多！的景点😊'
      }, {
        id: '0002',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1705/ed/edd4063a442f30c1a3.img.jpg_200x200_724f9e6a.jpg',
        title: '北京欢乐谷',
        desc: '近期小伙伴们收藏最！多！的景点😊'
      }, {
        id: '0003',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1705/ed/edd4063a442f30c1a3.img.jpg_200x200_724f9e6a.jpg',
        title: '北京欢乐谷',
        desc: '近期小伙伴们收藏最！多！的景点😊'
      }
      ]
    }
  }
}
</script>

<style lang="stylus" scoped>
  @import '~styles/mixins.styl'
  .title
    line-height: .8rem
    background: #eee
    text-indent: .2rem
    margin-top: .1rem
  .item
    overflow: hidden
    display: flex
    height: 1.9rem
    .item-img
      width: 1.7rem
      height: 1.7rem
      padding: .1rem
    .item-info
      flex: 1
      padding: .1rem
      min-width: 0
      .item-title
        line-height: .54rem
        font-size: .32rem
        ellipsis()
      .item-desc
        line-height: .4rem
        color: #ccc
        ellipsis()
      .item-button
        line-height: .44rem
        margin-top: .16rem
        background: #ff9300
        padding: 0 .2rem
        border-radius: .06rem
        color: #fff
</style>
