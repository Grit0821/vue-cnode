<template>
  <div id="app">
    <Header></Header>
    <div class="main">
      <router-view name="slidebar"></router-view>
      <router-view name="main"></router-view>
    </div>
  </div>
</template>

<script>
  // 引入用到的子组件
  import Header from './components/Header'
  import PostList from './components/PostList'
export default {
  name: 'App',
  components:{
    // 注入用到的子组件
    Header,
    PostList,
  }
}
</script>

<style>
.main{
  width: 80%;
  margin: 0 auto;
}
</style>
