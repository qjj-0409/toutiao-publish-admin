<template>
<!-- el-menu-item 的index不能重复，确保唯一即可 -->
<!-- router：是否使用 vue-router 的模式，启用该模式会在激活导航时以 index 作为 path 进行路由跳转 -->
<div>
<!-- <div class="aside-logo"></div> -->
<el-menu
  :default-active="$route.path"
  text-color="#fff"
  background-color="#002033"
  active-text-color="#ffd04b"
  router
  :collapse="isCollapse"
  class="aside-ul"
  >

  <el-menu-item index="/">
  <i class="el-icon-s-home"></i>
  <span slot="title">首页</span>
  </el-menu-item>
  <el-menu-item index="/article">
  <i class="el-icon-document"></i>
  <span slot="title">内容管理</span>
  </el-menu-item>
  <el-menu-item index="/image">
  <i class="el-icon-picture"></i>
  <span slot="title">素材管理</span>
  </el-menu-item>
  <el-menu-item index="/publish">
  <i class="el-icon-s-promotion"></i>
  <span slot="title">发布文章</span>
  </el-menu-item>
  <el-menu-item index="/comment">
  <i class="el-icon-chat-dot-round"></i>
  <span slot="title">评论管理</span>
  </el-menu-item>
  <el-menu-item index="/fans">
  <i class="el-icon-present"></i>
  <span slot="title">粉丝管理</span>
  </el-menu-item>
  <el-menu-item index="/setting">
  <i class="el-icon-setting"></i>
  <span slot="title">个人设置</span>
  </el-menu-item>
</el-menu>
</div>
</template>

<script>
export default {
  name: 'AppAside',
  props: ['isCollapse'],
  components: {},
  data () {
    return {}
  },
  computed: {},
  watch: {},
  methods: {},
  created () {},
  mounted () {},
  beforeDestroy () {}
}
</script>
<style lang='less' scoped>
.aside-ul {
  height: 100%;
}
// .aside-logo {
//   width: 100%;
//   height: 60px;
//   background: url(./logo_admin.png) no-repeat;
// }
</style>
