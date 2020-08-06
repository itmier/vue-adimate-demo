<!--
 * @Author: Tmier
 * @Date: 2020-08-06 21:36:33
 * @LastEditTime: 2020-08-06 22:05:34
 * @Description: 
-->
<template>
  <div id="app">
    <!-- <link href="https://cdn.jsdelivr.net/npm/animate.css@3.7.2" rel="stylesheet" type="text/css"> -->
    <el-button type="primary" @click="changeShow">变换</el-button>
    <div v-show="show" class="tmierShow animated bounce">HHH</div>
  </div>
</template>

<style lang="less">
html,body {
  width: 100%;
  height: 100%;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 100px;
  width:100%
}
.tmierShow {
  font-size: 50px;
  margin-top: 20px;
  width: 200px;
  height:60px;
  line-height: 60px;
  text-align: center;
  background: #000;
  color: #fff;
  margin: 50px auto;
}
</style>
<script>
// import 'animate.css/animate.min.css'
export default {
  data() {
    return {
      show:true
    }
  },
  methods: {
    changeShow() {
      this.show = !this.show
    }
  }
}
</script>
