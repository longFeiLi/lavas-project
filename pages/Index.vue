<template>
    <div class="page-index">
        <head-nav></head-nav>
        <h2>欢迎Lovell小窝</h2>
        <h4>如果你年轻时没有学会思考，那就永远学不会思考。</h4>
         <!-- link to index -->
        <router-link to="/detail/1">Back to Detail</router-link>
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
        title: 'Home',
        titleTemplate: 'lovell-有故事的网站',
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
