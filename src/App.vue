<template>
  <div id="app">
    <TopContainer></TopContainer>
    <BHeader></BHeader>
    <BContent></BContent>
  </div>
</template>

<script>
import TopContainer from 'components/common/TopContainer.vue';
import BHeader from 'components/common/BHeader.vue';
import BContent from 'components/content/BContent.vue';
import { mapGetters } from 'vuex';

export default {
  name: 'app',
  components: {
    TopContainer,
    BHeader,
    BContent
  }
}
</script>

<style lang="stylus">
  #app 
    font-family "Microsoft YaHei",Arial,Helvetica,sans-serif
    -webkit-font-smoothing antialiased
    font-size 12px
    margin 0
    padding 0
    background #fff
    color #222
    min-width 990px
    tap-highlight-color transparent
    -webkit-tap-highlight-color transparent
    .wnd-mask
      position fixed
      width 100%
      height 150%
      background-color #000
      opacity .5!important
      z-index 1000
      top 0px
      left 0px
      transition .2s
</style>