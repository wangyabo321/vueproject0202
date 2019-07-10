<template>
  <div class="home-wraper">
<!--    第一部分导航部分-->
    <div class="nav">
      <div class="nav-left"><i class="iconfont icon-jiantou1"></i></div>
      <div class="nav-content"><i class="iconfont icon-sousuo"></i><input type="search" placeholder="请输入搜索内容"></div>
      <div class="nav-right">三亚 <i class="iconfont icon-jiantou"></i></div>
    </div>
<!--    第二部分轮播图-->
    <div class="swiper-container">
      <swiper :options="swiperOption" ref="mySwiper">
        <!-- slides -->
        <swiper-slide><img src="../assets/images/banner-images/banner1.jpg" alt=""></swiper-slide>
        <swiper-slide><img src="../assets/images/banner-images/banner2.jpg" alt=""></swiper-slide>
        <swiper-slide><img src="../assets/images/banner-images/banner3.jpg" alt=""></swiper-slide>
        <swiper-slide><img src="../assets/images/banner-images/banner4.jpg" alt=""></swiper-slide>
        <swiper-slide><img src="../assets/images/banner-images/banner5.png" alt=""></swiper-slide>
        <!-- Optional controls -->
        <div class="swiper-pagination"  slot="pagination"></div>
      </swiper>
    </div>
<!--    第三部分字体图标列表-->



  </div>
</template>

<script>

export default {
  name: 'HelloWorld',
  data () {
    return {
      swiperOption: {
        loop:true,
        autoplay:true,
        pagination: {
          el: '.swiper-pagination',
        },
      }
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="stylus" scoped>
  .swiper-container >>> .swiper-pagination-bullet-active{
    background-color:#fff !important;
  }
  .nav{
    line-height:45px;
    width:100%;
    background:dodgerblue;
    display flex;
    color:#fff;
    text-align center
    .nav-left{
      width:50px;
      float:left;
      .icon-jiantou1{
        font-size:20px;
      }
    }
    .nav-content{
      flex:1;
      position:relative;
      i{
        color:#666;
        font-size:18px;
        position:absolute;
        top:1px;
        left:6px;
        z-index:1
      }
      input{
        width:100%;
        height:30px;
        border-radius:15px;
        text-indent:2em;
        position:absolute;
        left:0;
        top:8px;
      }
    }
    .nav-right{
      width:80px;
      float:right;
      .icon-jiantou{
        font-size:12px;
      }
    }
  }
  .swiper-container{
    img{
      width:100%;
    }
  }
</style>
