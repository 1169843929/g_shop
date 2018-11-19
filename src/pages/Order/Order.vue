<template>
    <section class="order">
        <HeaderTop title="订单列表"></HeaderTop>
        <section class="order-no-login">
            <img class="tips" src="./imgs/person.png" alt="">
            <h3>登录后查看外卖订单</h3>
            <button>立即登录</button>
        </section>
    </section>
</template>

<script>
import HeaderTop from '../../components/headerTop/headerTop.vue'
export default {
    components:{
        HeaderTop,
    }
}
</script>

<style lang="stylus" rel="stylesheet/styls">
    @import "../../commen/stylus/mixins.styl"
    .order
        text-align center
        .order-no-login
            font-size 12px
            width 50%
            margin 0px auto 
            text-align center
            .tips
                margin-top 80%
                width 100%
            h3
                color #333333
                margin-top 5px
            button 
                margin-top 20px
                padding 5px
                color #eee
                background #02a774
                border: 1px solid transparent;  
                outline: none;    //消除默认点击蓝色边框效果
                border-radius 4px
</style>
