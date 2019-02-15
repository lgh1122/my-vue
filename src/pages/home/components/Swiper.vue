<template>
  <div class="wrapper">
    <swiper :options="swiperOption">
      <!-- slides -->
      <swiper-slide v-for="item of SwiperList" :key="item.id">
        <img class="swiper-img" :src="item.imgUrl">
      </swiper-slide>

      <!-- Optional controls -->
      <div class="swiper-pagination"  slot="pagination"></div>
      <!--<div class="swiper-button-prev" slot="button-prev"></div>
      <div class="swiper-button-next" slot="button-next"></div>
      <div class="swiper-scrollbar"   slot="scrollbar"></div>-->
    </swiper>
  </div>
</template>
<script>
export default {
  name: 'HomeSwiper',
  data () {
    return {
      swiperOption: {
        pagination: 'swiper-pagination',
        loop: true
      },
      SwiperList: [
        {
          id: '0001',
          imgUrl: 'http://img1.qunarzz.com/piao/fusion/1712/d0/0f5f1844045c0102.jpg_890x330_68cb5860.jpg'
        }, {
          id: '0002',
          imgUrl: 'http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20192/3204f6960133ada839a24fc7781ab310.jpg_890x330_01abe7cc.jpg'
        }
      ]
    }
  }
}
</script>
<style lang="stylus" scoped>
  .wrapper >>> .swiper-pagination-bullet-active
    background #23231F
  .wrapper
    overflow hidden
    width 100%
    height 0
    padding-bottom 32.25%
    background #eee
    .swiper-img
      width 100%
</style>
