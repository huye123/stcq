<template>
  <div class="hello">
    <van-nav-bar fixed class="index">
      <div slot="left">
        <!-- <span class="title">生态新青</span> -->
        <van-col span="4">span: 4</van-col>
        <img src="../../static/image/logo.png" alt="">
      </div>
  <van-icon name="search" slot="right" />
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


</style>
