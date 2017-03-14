<template>
  <div id="app">
    <descTop></descTop>
    <ul class="home_nav">
      <li><a href="javascript:;" class="selected">直播</a></li>
      <li><a href="javascript:;">群成员</a></li>
      <li><a href="javascript:;">更多精彩</a></li>
    </ul>
    <liveList></liveList>
    <a href="javascript:;" class="join_circle">加入社群</a>
  </div>
</template>

<script>
  import 'common/css/reset.css';
  import 'common/js/reset.js';
  import DescTop from 'components/DescTop/DescTop.vue';
  import LiveList from 'components/LiveList/LiveList.vue'

  export default {
    name: 'app',
    components: {
      DescTop,LiveList
    }
  }
</script>

<style>
  #app {
    font-family: "Microsoft YaHei UI";
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
  }
  .home_nav{background: #fff; height: 0.79rem; line-height: 0.79rem; border-bottom: #e6e6e6 solid 1px;}
  .home_nav li{width: 33.333%; float: left; text-align: center; height: 0.79rem; line-height: 0.79rem; font-size: 0.3rem;}
  .home_nav li a{color: #323232; line-height: 0.75rem; font-size: 0.3rem; padding: 0 0.06rem; display: inline-block;}
  .home_nav li a.selected{color: #fd2a2a; border-bottom: #fd2a2a solid 4px;}
  .join_circle{position: fixed; left: 0; bottom: 0; width: 100%; height: 0.96rem; line-height: 0.96rem;background: #ff3838; font-size: 0.34rem; color: #fff;}
</style>
