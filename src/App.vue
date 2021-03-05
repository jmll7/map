<template>
  <div id="app">
    <!--    <img src="./assets/logo.png">-->
    <div id="container" class="container"> </div>
    <!--    <HelloWorld/>-->
  </div>
</template>

<script>
  import HelloWorld from './components/HelloWorld'

  export default {
    name: 'App',
    components: {
      HelloWorld
    },
    mounted() {
      this.initMap();
    },
    methods: {
      initMap() {
        this.map = new AMap.Map('container', {
          zoom:11,//级别
          center: [118.92137, 32.10467]//中心点坐标
        });
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
  .container {
  / / 容器大小
    /*margin-left: %;*/
  width: 100%;
    height: 850px;
  }
</style>
