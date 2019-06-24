<template>
  <div id="app">
  <ppm-projectAccess></ppm-projectAccess>
  <ppm-productAccess></ppm-productAccess>
  <ppm-strategyAccess></ppm-strategyAccess>
  </div>
</template>

<script>
import projectAccess from './Components/projectAccess/projectAccess'
import productAccess from './Components/productAccess/productAccess'
import strategyAccess from './Components/strategyAccess/strategyAccess'
export default {
  components:{
    'ppm-projectAccess':projectAccess,
    'ppm-productAccess':productAccess,
    'ppm-strategyAccess':strategyAccess
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
