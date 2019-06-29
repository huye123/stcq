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
<van-swipe @change="onChange">
  <van-swipe-item>1</van-swipe-item>
  <van-swipe-item>2</van-swipe-item>
  <van-swipe-item>3</van-swipe-item>
  <van-swipe-item>4</van-swipe-item>

  <div class="custom-indicator" slot="indicator">
    {{ current + 1 }}/4
  </div>
</van-swipe>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
       current: 0
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

</style>
