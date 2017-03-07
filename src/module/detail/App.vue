<template>
  <div id="app">
    <img src="./images/logo.png">
    <div>详情内容</div>
    <video-player :options="videoOptions" @player-state-changed="playerStateChanged"></video-player>
  </div>
</template>

<script>
  import 'common/css/reset.css';
  import Hello from 'components/Hello/Hello'
  import VideoPlayer from 'vue-video-player';
  VideoPlayer.config({
    youtube: false,
    switcher: true,
    hls: true
  })
  export default {
    name: 'app',
    components: {
      Hello,
      VideoPlayer
    },
    data () {
      return {
        videoOptions: {
          source: {
            type: "application/x-mpegURL",
            src: 'https://logos-channel.scaleengine.net/logos-channel/live/biblescreen-ad-free/playlist.m3u8',
            withCredentials: false
          },
          language: 'zh-CN',
          live: true,
          autoplay: true,
          height: 540
        }
      }
    },
    methods: {
      playerStateChanged(playerCurrentState) {
        console.log(playerCurrentState)
      }
    }
  }
</script>

<style>
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }
</style>
