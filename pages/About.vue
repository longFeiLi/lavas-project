<template>
    <div class="page-index">
        <head-nav></head-nav>
        <h2>关于我们</h2>
        <h4>作者:longfeili0925@gmail.com</h4>
    </div>
</template>

<script>
import HeadNav from '@/components/Header';
function setState(store) {}

export default {
    name: 'index',
    components: {
      HeadNav
    },
    metaInfo: {
        title: 'About',
        titleTemplate: 'lovell-关于我们',
        meta: [
            {name: 'keywords', content: 'lovell love longfei ,feifei,龙飞 龙飞小窝 龙飞Lovell'},
            {name: 'description', content: 'lovell分享各种经典句子，个人学习心得体会'}
        ]
    },
    async asyncData({store, route}) {
        setState(store);
    }
};
</script>

<style lang="stylus" scoped>

.page-index
    display flex
    justify-content center
    align-items center
    flex-direction column

    h2
        font-size 46px
        font-weight 500
        color: #096DD9
        margin-bottom 0


    font-family: Lato, "Monospaced Number", "Chinese Quote", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "PingFang SC", "Hiragino Sans GB", "Microsoft YaHei", "Helvetica Neue", Helvetica, Arial, sans-serif;

</style>
