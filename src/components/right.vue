<template>
<div id = 'weathers'>
<app-weather>{{weather}}</app-weather>
 </div>
</template>
<script>

import Head from './head.vue'
export default {
components:{
    'app-weather': Head
},
props:['weather']
    
}
</script>
<style  scoped>
#weathers{
   color: blue;
   float: right;
   width: 35%;
   background-color: black;
}
</style>