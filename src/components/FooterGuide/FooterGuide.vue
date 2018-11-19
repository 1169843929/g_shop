<template>
    <div class="footer-guide">
        <span class="guide-item" :class="{on:'/msite'===$route.path}" @click="GoTo('/msite')">
            <span class="item-icon">
                <i class="iconfont icon-u"></i>
            </span>
            <p>外卖</p>
        </span>
        <span class="guide-item" :class="{on:'/search'===$route.path}" @click="GoTo('/search')">
            <span class="item-icon">
                <i class="iconfont icon-sousuo1"></i>
            </span>
            <p>搜索</p>
        </span>
        <span class="guide-item" :class="{on:'/order'===$route.path}" @click="GoTo('/order')">
            <span class="item-icon">
                <i class="iconfont icon-dingdan"></i>
            </span>
            <p>订单</p>
        </span>
        <span class="guide-item" :class="{on:'/profile'===$route.path}" @click="GoTo('/profile')">
            <span class="item-icon">
                <i class="iconfont icon-gerenkuang"></i>
            </span>
            <p>我的</p>
        </span>
    </div>
</template>

<script>
export default {
    methods:{
        GoTo(path){
            //$route和$router的区别
            // this.$router 实际上 就是全局 路由对象  任何页面 都可以 调用 push(), go()等方法
            // this.$route  表示当前正在用于跳转的路由器对象，可以调用其name、path、query、params等属性;
            this.$router.replace(path)
        }
    }
}
</script>

<style lang="stylus" rel="stylesheet/stylus">
@import "../../commen/stylus/mixins.styl"
    .footer-guide
        top-border-1px(#e4e4e4)
        position fixed
        z-index 100
        bottom  0
        left 0
        right 0
        background #ffffff
        width 100%
        height  50px
        display flex
        color #333
        .guide-item
            width 25%
            text-align center
            margin-top 5px
            font-size 14px
        .on
            color #02a774


</style>
