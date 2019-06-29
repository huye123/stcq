<template>
  <div class="hello">
    <van-nav-bar fixed class="index">
      <div slot="left">
        <!-- <span class="title">生态新青</span> -->
        <van-col span="8" class="logo">
          <img src="../../static/image/logo.png" alt="">
        </van-col>
        <van-col span="12" class="indexBtn" :offset="2">
         <button>景点</button>
        </van-col>
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
   background-color: rgba(25, 186, 117, 0.5);
   /* opacity: 0.5; */
 
 }
  .logo img{
     width: 100%;
      display: block;
      margin-top: 10px;

   }
   .indexBtn button{
     background-color: #65b696;
     border: 0px;
    width: 100%;
    border-radius: 25px;
   }

</style>
