<template>
  <div class="home-wraper">
    <div class="nav-left"><i class="iconfont icon-jiantou1"></i></div>
    <div class="nav-content"><i class="iconfont icon-sousuo"></i><input type="search" placeholder="请输入搜索内容"></div>
    <div class="nav-right">三亚 <i class="iconfont icon-jiantou"></i></div>

<!--    <span class="iconfont icon-jiantou"></span>-->
  </div>
</template>

<script>

export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="stylus" scoped>
  .home-wraper{
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
</style>
