<template>
  <div id="app">
  <ppm-controls v-bind:accessData="projectAccessData"></ppm-controls>
  <ppm-controls v-bind:accessData="resourceAccessData"></ppm-controls>
  <ppm-controls v-bind:accessData="strategyAccessData"></ppm-controls>
  </div>
</template>

<script>
import controls from './Components/commonControls/controls'
import accessData from './data/projectAccess.js'
export default {
  data:function(){
    return accessData
    },
  components:{
    'ppm-controls':controls
  }
}
</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
