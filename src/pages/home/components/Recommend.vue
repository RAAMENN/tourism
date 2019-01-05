<template>
  <div>
    <div class="recommend-title">推荐</div>
    <ul>
      <li class="recommend-item border-bottom" v-for="item of recommendList" :key="item.id">
        <img :src="item.imgUrl" class="item-img">
        <div class="item-info">
          <p class="item-title">{{item.title}}</p>
          <p class="item-desc">{{item.desc}}</p>
          <button class="item-button">查看详情</button>
        </div>
      </li>
    </ul>
  </div>
</template>

<script type='text/ecmascript-6'>
export default {
  name: 'HomeRecommand',
  data () {
    return {
      recommendList: [{
        id: '0001',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1712/95/95f38f28a6ff19cba3.img.jpg_200x200_af967e35.jpg',
        title: '水奥雪世界',
        desc: 'desc'
      }, {
        id: '0002',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1712/95/95f38f28a6ff19cba3.img.jpg_200x200_af967e35.jpg',
        title: '水奥雪世界',
        desc: 'desc'
      }, {
        id: '0003',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1712/95/95f38f28a6ff19cba3.img.jpg_200x200_af967e35.jpg',
        title: '水奥雪世界',
        desc: 'desc'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
  @import "~styles/mixins.styl"

  .recommend-title
    margin-top: .2rem
    line-height: .8rem
    background: #eee
    text-indent: .2rem
  .recommend-item
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
      min-width: 0 //why?
      .item-title
        line-height: .54rem
        font-size : .32rem
        ellipsis()
      .item-desc
        line-height: .4rem
        color: #ccc
        ellipsis()
      .item-button
        margin-top: .16rem
        background: #ff9300
        padding: 0 .2rem
        border-radius: .06rem
        color: #fff
        line-height: .44rem
</style>
