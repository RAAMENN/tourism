<template>
  <div class="header">城市选择
    <router-link to="/">
      <div class="header-left">
        <div class="iconfont header-back">&#xe624;</div>
      </div>
    </router-link>
  </div>
</template>

<script type='text/ecmascript-6'>
export default {
  name: 'CityHeader'
}
</script>

<style lang="stylus" scoped>
  @import "~styles/varibles.styl"
.header
  height: $headerHeight
  line-height : $headerHeight
  overflow :hidden
  text-align :center
  color : #fff
  background : $bgColor
  font-size: .32rem
  position : relative
  .header-back
    position : absolute
    top: 0
    left: 0
    width : .64rem
    text-align : center
    font-size : .4rem
    color : #fff
</style>
