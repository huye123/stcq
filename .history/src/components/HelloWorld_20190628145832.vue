<template>
  <div class="hello">
    <van-nav-bar fixed class="index">
      <div slot="left">
        <!-- <span class="title">生态新青</span> -->
        <van-col span="8" class="logo">
          <img src="../../static/image/logo.png" alt="">
        </van-col>
        <van-col span="8" class="indexBtn"></van-col>
        <van-button round type="danger">圆形按钮</van-button>
      </div>
  <!-- <van-icon name="search" slot="right" /> -->
</van-nav-bar>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
     
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->

<style scoped>
 .index{
   background: #19ba75;
   opacity: 0.5;
 
 }
  .logo img{
     width: 100%;
      display: block;
      margin-bottom: 10px;
   }

</style>
