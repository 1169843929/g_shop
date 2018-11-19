<template>
    <section class="profile">
        <HeaderTop title="我的"></HeaderTop>
        <section class="login">
            <span class="header-img">
                <i class="iconfont icon-geren"></i>
            </span>
            <router-link to="/login" class="log">
                <span>
                    <span class="goto">登录/注册</span>
                    <p class="number"><i class="iconfont icon-shouji"></i>暂无绑定手机号</p>
                </span>
                <span class="jiantou">
                    <i class="iconfont icon-z043"></i>
                </span>
            </router-link>
            
        </section>
        <section class="userInformation">
            <span class="myMoney">
                <p><span class="number1">0.00</span>元</p>
                <p>我的余额</p>
            </span>
            <span class="favourable">
                <p><span class="number2">0</span>个</p>
                <p>我的优惠</p>
            </span>
            <span class="integration">
                <p><span class="number3">0</span>分</p>
                <p>我的积分</p>
            </span>
        </section>
        <section class="something">
            <div class="userOrder">
                <span class="myOrderIcon"><i class="iconfont icon-order"></i></span>
                <span class="myOrder">
                    <span style="colo">我的订单</span>
                    <span style="">></span>
                </span>
            </div>
            <div class="integrationShop">
                <span class="myOrderIcon"><i class="iconfont icon-jifen"></i></span>
                <span class="myOrder">
                    <span>积分商城</span>
                    <span>></span>
                </span>
            </div>
            <div class="membershipCard">
                <span class="myOrderIcon"><i class="iconfont icon-huiyuan1"></i></span>
                <span class="myOrder">
                    <span>硅谷外卖会员卡</span>
                    <span>></span>
                </span>
            </div>
        </section>
        <section class="serviceCenter">
            <span class="myOrderIcon"><i class="iconfont icon-service"></i></span>
            <span class="myOrder">
                <span>服务中心</span>
                <span>></span>
            </span>
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
    .profile
        text-align center
        width 100%
        height 100%
        overflow hidden
        .login
            margin-top 45px
            height 15%
            border-top 2px solid #02ad74
            background #02a774
            // padding 15px 5px
            display flex
            flex-wrap wrap
            align-items center
            .header-img
                width 15%
                border-radius 50%
                margin 0 4%
                .icon-geren
                    font-size 40px
                    color #aaa  
                    background #eeeeee
                    
            .log
                width 75%
                position relative
                color #ffffff
                text-align  left 
                .goto
                    font-size 16px
                .number
                    font-size 12px
                .jiantou
                    position absolute
                    right 10px
                    top 40%
                    color #eeeeee
        .userInformation
            display flex
            width 100%
            height 70px
            background white
            color #333333
            align-items center
            font-size 12px
            .myMoney
                width 33%
                .number1
                    color #F5A100
                    font-size 20px
                    font-weight bold
                p:nth-child(2)
                    color #777777
            .favourable
                width 33%
                .number2
                    color #02a774
                    font-size 20px
                    font-weight bold
                p:nth-child(2)
                    color #777777
            .integration
                width 33%
                .number3
                    color #F5A100
                    font-size 20px
                    font-weight bold
                p:nth-child(2)
                    color #777777
        .something
            width 100%
            height 140px
            background white
            color #555555
            font-size 14px
            margin-top 10px
            .userOrder
                height 33%
                display flex
                align-items center
                border-bottom 1px solid #dddddd
                .myOrderIcon
                    width 7%
                    color #02a774
                .myOrder
                    width 93%
                    text-align left
                    span:nth-child(2)
                        float right
                        margin-right 5%
                        color #999
            .integrationShop
                height 33%
                display flex
                align-items center
                border-bottom 1px solid #dddddd
                .myOrderIcon
                    width 7%
                    color red
                .myOrder
                    width 93%
                    text-align left 
                    span:nth-child(2)
                        float right
                        margin-right 5%
                        color #999
            .membershipCard
                height 33%
                display flex
                align-items center
                .myOrderIcon
                    width 7%
                    color #F5A100
                .myOrder
                    width 93%
                    text-align left 
                    span:nth-child(2)
                        float right
                        margin-right 5%
                        color #999
        .serviceCenter
            width 100%
            height 46px
            background white
            color #555555
            font-size 14px
            margin-top 10px
            display flex
            align-items center
            .myOrderIcon
                width 7%
                color #02a774
            .myOrder
                width 93%
                text-align left 
                span:nth-child(2)
                    float right
                    margin-right 5%
                    color #999

                    
</style>
