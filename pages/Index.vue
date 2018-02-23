<template>
    <div class="page-index">
        <h2>LAVAS</h2>
        <h4>test环境</h4>
         <!-- link to index -->
        <router-link to="/detail/1">Back to Detail</router-link>
    </div>
</template>

<script>
function setState(store) {}

export default {
    name: 'index',
    metaInfo: {
        title: 'Home',
        titleTemplate: '我的标题',
        meta: [
            {name: 'keywords', content: 'lavas PWA'},
            {name: 'description', content: '解决各种电影票价问题'}
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
        margin-bottom 0

</style>
