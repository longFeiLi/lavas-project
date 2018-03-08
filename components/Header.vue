<template>
	 <div class="head">
	   <div class="logo">
	      <a href="//www.lovell.com.cn">
	        <img src="../assets/img/logo.png" style="height:50px;">
	      </a>
	   </div>
	   <nav class="nav-list">
	      <ul>
	        <li v-bind:class="{ active: $route.path === '/' }">
	        	 <router-link to="/" >
               Home
            </router-link>
	        </li>
	        <li>
              <router-link to="/list">列表</router-link>
          </li>
	        <li>
              <router-link to="/counter" >资料</router-link>
          </li>
	        <li v-bind:class="{ active: $route.path === '/about' }">
            <router-link to="/about" >关于</router-link>
          </li>
	      </ul>
	   </nav>
	 </div>
</template>
<script>
  export default {
    computed: {
    },
    // 定义变量
    data () {
      return {
      }
    },
    // 引入组件
    props: {},
    mounted: function () {
    },
    // 方法
    methods: {
    },
    components: {
    }
  }
</script>
<style lang="stylus" scoped>
.head
   height 60px
   position fixed
   line-height 60px
   top 0
   left 0
   width 100%
   padding 0 5%
   display flex
   box-sizing border-box;
   box-shadow 0 2px 8px #f0f1f2
   transition all 0.3s
   background-color #FFF
   a 
     color #1890ff
     text-decoration none
     cursor: pointer;
   .logo
      width 120px
      line-height 60px
      font-size 22px
      font-weight bold
      padding: 5px 0px;
      margin-right 20px
   .nav-list
     margin-left 20px
     ul
       list-style-type none
       display flex
       margin 0px
       li
          width 70px
          font-size 14px
          a
            color #314659

       .active
          border-top: 2px solid #1890ff
          a
            color: #1890ff
            font-size 16px
            font-weight 500


</style>
