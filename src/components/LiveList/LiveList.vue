<template>
  <div class="live_main">
    <div class="no_data">
      群主还在马不停蹄，准备直播内容中
    </div>
    <div class="live_list_con">
      <p class="live_more"><a href="javascript:;">查看全部直播</a>&gt;</p>
      <ul class="live_list">
        <li>
          <div class="lt_img">
            <img src="">
            <p class="red">直播</p>
            <p class="video_ioc"></p>
          </div>
          <div class="lt_text">
            <p class="title">东寨港红树林，沿着李克强总理的足迹感受不一样的海上森林</p>
            <div class="lt_time">
              <p>2017-02-12 10:21 </p>
              <p>128</p>
            </div>
          </div>
        </li>
      </ul>
    </div>
  </div>
</template>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .live_main{overflow: hidden; overflow-y: auto;}
  .no_data{width: 100%; background: url("../../module/index/images/no_data_ioc.png") no-repeat center 1.12rem; background-size: 2.04rem 2.32rem; font-size: 0.28rem; color: #a0a0a0; text-align: center; padding-top: 4.04rem; padding-bottom: 1rem;}
  .live_list_con{}
  .live_more{height: 0.7rem; line-height: 0.7rem; text-align: center; font-size: 0.28rem; background: #f5f5f5;}
  .live_more a{color: #565656; padding-right: 0.32rem;}
  .live_list{padding: 0.3rem;}
  .live_list li{display: -webkit-box;}
  .lt_img{width: 2.4rem; height: 1.5rem; position: relative; float: left;}
  .lt_img p:nth-child(2){width: 0.44rem; height: 0.24rem; line-height: 0.24rem; font-size: 0.18rem; color: #fff; text-align: center; position: absolute; top:0.1rem; left: 0.1rem;}
  .lt_img p.red{background: #f01414;}
  .lt_img p.blue{background: #3c8cfa;}
  .lt_img p.orgin{background: #ff9600;}
  .lt_img p:nth-child(3){width: 0.28rem; height: 0.28rem; border-radius: 100%; position: absolute; right: 0.08rem; bottom: 0.08rem;}
  .video_ioc{background: rgba(0,0,0,0.4) url("../../module/index/images/g_ioc_3.png") no-repeat; background-size: 0.28rem 0.28rem;}
  .aideo_ioc{background: rgba(0,0,0,0.4) url("../../module/index/images/g_ioc_4.png") no-repeat; background-size: 0.28rem 0.28rem;}
  .lt_text{padding-left: 0.22rem; -webkit-box-flex: 1;}
  .lt_text .title{font-size: 0.28rem; line-height: 0.36rem; color: #323232;}
  .lt_time{height: 0.22rem; padding-top: 0.42rem;}
  .lt_time p{padding-left: 0.32rem; height: 0.22rem; font-size: 0.24rem; color: #a0a0a0;}
  .lt_time p:nth-child(1){width: 2.3rem; float: left;background: rgba(0,0,0,0.4) url("../../module/index/images/g_ioc_5.png") no-repeat; background-size: 0.28rem 0.28rem;}
  .lt_time p:nth-child(2){float: right;background: rgba(0,0,0,0.4) url("../../module/index/images/g_ioc_6.png") no-repeat; background-size: 0.28rem 0.28rem;}
</style>
