<template>
  <div id="app">
    <!-- 路由渲染,网页路径指向哪个组件就渲染哪个组件 -->
    <router-view/>
    <FooterGuide v-show="$route.meta.showFooter==true"/>
  </div>
</template>

<script>
import FooterGuide from './components/FooterGuide/FooterGuide.vue'
export default {
  components:{
    FooterGuide
  }
}
</script>

<style lang="stylus" rel="stylesheet/stylus">
//  用stylus格式来写css
#app 
  width 100%
  height 100%
  background #f5f5f5
</style>
