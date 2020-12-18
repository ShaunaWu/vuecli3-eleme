<template>
  <div class="title-wrapper">
    <div class="info">
      <img class="avatar" src="http://static.galileo.xiaojukeji.com/static/tms/seller_avatar_256px.jpg" alt="">
      <div class="desc">
        <div class="title">
          <span class="brand"></span>
          <span class="name">粥品香坊(大运村)</span>
        </div>
        <div class="time">
          蜂鸟专送/38分钟送达
        </div>
        <div class="discount">
          <support-ico size=1 type=0></support-ico>
          <div class="text">在线支付满28减5，满50减10</div>          
        </div>
      </div>
      <div class="count">
        <span class="amount">5个</span>
        <i class="icon-keyboard_arrow_right"></i>
      </div>
    </div>
    <div class="bulletin">
      <span class="title"></span>
      <span class="desc">粥品在线支付满28减5，满50减10在线支付满28减5，满50减10在线支付满28减5，满50减10</span>
      <i class="icon-keyboard_arrow_right"></i>
    </div>
    <div class="background">
      <img src="http://static.galileo.xiaojukeji.com/static/tms/seller_avatar_256px.jpg" width="100%">
    </div>
  </div>
</template>

<script>

import supportIco from '../support-ico/support-ico'

export default {

  name: 'v-header',
  components: {
    supportIco
  },
  props: {

  }
}
</script>

<style lang="stylus" scoped>

  @import "../../common/stylus/mixin"
  @import "../../common/stylus/variable"

  .title-wrapper
    width 100%
    background-color $color-background-ss
    .info
      display flex
      position relative
      padding 24px 12px 18px 24px
      .avatar
        flex 0 0 64px
        width 64px
        height 64px        
        margin-right 16px
        border-radius 2px
      .desc
        flex 1
        .title
          display flex
          align-items center
          padding-top 2px
          .brand
            width 30px
            height 18px
            background-size 30px 18px
            margin-right 6px
            bg-image('brand')
          .name
            font-size 16px
            color rgb(255, 255, 255)
            font-weight bold
            line-height 18px
        .time
          margin-top 8px
          font-size 12px
          color rgb(255, 255, 255)
          font-weight 200
          line-height 12px
        .discount
          display flex
          margin-top 10px
          margin-bottom 2px
          .text
            margin-left 4px
            font-size 10px
            color rgb(255, 255, 255)
            font-weight 200
            line-height 12px
      .count
        position absolute
        display flex
        right 12px
        bottom 18px
        font-size 10px
        color rgb(255, 255, 255)
        font-weight 200
        line-height 12px
        padding 7px 8px
        border-radius 16px
        background-color rgba(0, 0, 0, 0.2)
        .amount
          margin-right 2px
    .bulletin
      display flex
      align-items center
      padding 0 8px
      background-color $color-background-sss
      .title
        flex 0 0 22px
        width 22px
        height 12px
        background-size 22px 12px
        margin-right 6px
        bg-image('bulletin')
      .desc
        flex 1
        font-size 10px
        color rgb(255, 255, 255)
        font-weight 200
        line-height 28px
        margin 0 4px
        white-space nowrap
        overflow hidden
        text-overflow ellipsis
      .icon-keyboard_arrow_right
        flex 0 0 10px
        color rgb(255, 255, 255)
    .background
      position absolute
      top 0
      left 0
      width 100%
      z-index -1
      filter: blur(10px)
</style>