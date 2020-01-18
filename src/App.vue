<template>
  <div id="app">
    <!-- 显示的是当前路由地址所对应的内容 -->
    <keep-alive exclude="Detail">
      <router-view/>
    </keep-alive>
    <home></home>
  </div>
</template>

<script>
import Home from '@/pages/home/Home'
export default {
  name: 'App',
  components:{
    Home
  }
}
</script>

<style>

</style>
