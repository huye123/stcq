<template>
  <div class="hello">
    <van-nav-bar fixed class="index">
      <div slot="left">
        <!-- <span class="title">生态新青</span> -->
        <van-col span="8" class="logo">
          <img src="../../static/image/logo.png" alt="">
        </van-col>
        <router-link :to="search">
          <van-col span="14" class="indexBtn" :offset="1">
            <button>景点</button>
          </van-col>
        </router-link>
      </div>
  <!-- <van-icon name="search" slot="right" /> -->
</van-nav-bar>
  </div>
</template>