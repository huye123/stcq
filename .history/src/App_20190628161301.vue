<template>
  <div id="app">
  <van-tabbar v-model="active">
  <van-tabbar-item >
    <span>推荐</span>
    <img
      slot="icon"
      slot-scope="props"
      :src="props.active ? icon.active : icon.normal"
    >
  </van-tabbar-item>
  <van-tabbar-item >
    <span>导航</span>
    <img
      slot="iconNav"
      slot-scope="search"
      :src="search.active ? iconNav.active : iconNav.normal"
    >
  </van-tabbar-item>
  <!-- <van-tabbar-item icon="search">标签</van-tabbar-item>
  <van-tabbar-item icon="setting-o">标签</van-tabbar-item>
  <van-tabbar-item icon="search">标签</van-tabbar-item> -->
</van-tabbar>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      active: 0,
      icon: {
        normal: 'static/image/tuijian-n.png',
        active: 'static/image/tuijian-s.png'
      },
       iconNav: {
        normal: 'static/image/daolan-n.png',
        active: 'static/image/daolan-s.png'
      }
    }
  },
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
