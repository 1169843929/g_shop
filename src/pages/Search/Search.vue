<template>
    <section class="search">
        <HeaderTop title="搜索"></HeaderTop>
        <section class="find">
            <input type="text" class="push" placeholder="请输入关键字">
            <input type="submit" value="提交" class="send">
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
    .search
        overflow hidden
        width 100%
        height 100%
        text-align center
        .find 
            margin-top 45px
            background #ffffff
            padding 10px
            .push
                width 80%
                background #eee
                outline none 
                padding 5px
                border-radius 2px
            .send
                width 15%
                padding 5px 5px
                background #02a774
                border 1px solid transparent
                border-radius 5px
                outline none 
</style>
