<template>
  <div id="app">
    <app-test></app-test>
  
  </div>
</template>
<script>
//import head from './components/head.vue'
import test from './components/test'

export default {
  name: 'App',
  components: {
    //'app-head': head,
    'app-test': test
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
