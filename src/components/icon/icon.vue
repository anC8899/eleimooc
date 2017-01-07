<template>
   <span class="icon" :class="iconType"></span>
</template>
<style lang="stylus" rel="stylesheet/stylus">
  @import "../../common/stylus/mixin"
  .icon
    display: inline-block
    background-repeat: no-repeat
    &.icon_1
      width: 12px
      height: 12px
      background-size: 12px 12px;
    &.decrease_1
      bg-image('decrease_1')
    &.discount_1
      bg-image('discount_1')
    &.guarantee_1
      bg-image('guarantee_1')
    &.invoice_1
      bg-image('invoice_1')
    &.special_1
      bg-image('special_1')
    &.icon_2
      width: 16px
      height: 16px
      background-size: 16px 16px;
    &.decrease_2
      bg-image('decrease_2')
    &.discount_2
      bg-image('discount_2')
    &.guarantee_2
      bg-image('guarantee_2')
    &.invoice_2
      bg-image('invoice_2')
    &.special_2
      bg-image('special_2')
    &.icon_3
      width: 12px
      height: 12px
      background-size: 12px 12px;
    &.decrease_3
      bg-image('decrease_3')
    &.discount_3
      bg-image('discount_3')
    &.guarantee_3
      bg-image('guarantee_3')
    &.invoice_3
      bg-image('invoice_3')
    &.special_3
      bg-image('special_3')
    &.icon_4
      width: 16px
      height: 16px
      background-size: 16px 16px;
    &.decrease_4
      bg-image('decrease_4')
    &.discount_4
      bg-image('discount_4')
    &.guarantee_4
      bg-image('guarantee_4')
    &.invoice_4
      bg-image('invoice_4')
    &.special_4
      bg-image('special_4')

</style>
<script type="text/ecmascript-6">
    export default{
      props: {
        size: {
          type: Number
        },
        type: {
          type: Number
        }
      },
      computed: {
        iconType () {
          return 'icon_' + this.size + ' ' + this.classMap[this.type] + '_' + this.size;
        }
      },
      created () {
        this.classMap = ['decrease', 'discount', 'special', 'invoice', 'guarantee'];
      }
    };
</script>
