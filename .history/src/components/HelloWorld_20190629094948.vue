<template>
  <div class="hello">
    <van-nav-bar fixed class="index">
      <div slot="left">
        <!-- <span class="title">生态新青</span> -->
        <van-col span="6" class="logo">
          <img src="../../static/image/logo.png" alt="">
        </van-col>
        <router-link :to="{ name: '搜索'}">
          <van-col span="15" class="indexBtn" :offset="2">
            <button>景点</button>
          </van-col>
        </router-link>
      </div>
  <!-- <van-icon name="search" slot="right" /> -->
</van-nav-bar>
<!-- 轮播 -->
<van-swipe @change="onChange" class="banner">
  <van-swipe-item><img :src="banner.imgFirst"></van-swipe-item>
  <van-swipe-item><img :src="banner.imgSecond"></van-swipe-item>
  <!-- <van-swipe-item><img :src="banner.imgThird"></van-swipe-item>
  <van-swipe-item><img :src="banner.imgFourth"></van-swipe-item> -->

  <!-- <div class="custom-indicator" slot="indicator">
    {{ current + 1 }}/4
  </div> -->
</van-swipe>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
       current: 0,
       banner:{
         imgFirst:'../static/image/banner.png',
         imgSecond:'../static/image/banner.png',

       }
       
    }
  },
    methods: {
    onChange(index) {
      this.current = index;
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->

<style scoped>
 .index{
   background-color: rgba(25, 186, 117, 0.5);
   /* opacity: 0.5; */
 
 }
  .logo img{
     width: 100%;
      display: block;
      margin-top: 12px;

   }
   .indexBtn button{
     background-color:  rgba(105, 184, 153, 0.5);
     border: 0px;
     width: 100%;
     border-radius: 25px;
     line-height: 30px;
     color: #fff;
     text-align: left;
     padding-left: 20px;
   }
  .banner img{
  width: 100%;
  }
  .van-swipe{
    
  }
</style>
