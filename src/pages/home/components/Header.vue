<template>
  <div class="header">
    <div class="header-left">
      <div class="iconfont backicon">&#xe624;</div>
    </div>
    <div class="header-input">
      <span class="iconfont input-icon">&#xe632;</span>
      输入城市/景点/游玩主题
    </div>
    <div class="header-right">
      城市
      <span class="iconfont arrow-icon">&#xe6aa;</span></div>
  </div>
</template>
<script>
export default {
  name: 'HomeHeader'
}
</script>
<style lang="stylus" scoped>
  @import "~@/assets/styles/varibles.styl"
  .header
    display: flex
    background: $bgColor
    color: #fff
    line-height: .86rem
    .header-left
      width: .64rem
      float: left
      text-align: center
      .backicon
        font-size: .4rem
        text-align: center
    .header-input
      flex: 1
      background: #fff
      height: .64rem
      line-height: .64rem
      border-radius: .1rem
      margin-top: .12rem
      margin-left: .2rem
      color: #ccc
      .input-icon
        font-size: .3rem
    .header-right
      width: 1.24rem
      float: right
      text-align: center
      .arrow-icon
        margin-left: -.04rem
        font-size: .24rem

</style>
