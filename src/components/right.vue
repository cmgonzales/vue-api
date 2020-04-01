<template>
<app-weather>{{info}}</app-weather>
 
</template>
<script>

import Head from './head.vue'
export default {
components:{
    'app-weather': Head
}
    
}
</script>