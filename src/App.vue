<template>
  <div id="app">
    <app-head></app-head>
  
  </div>
</template>
<script>
import head from './components/head.vue'


export default {
  name: 'App',
  components: {
    'app-head': head,

  
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
