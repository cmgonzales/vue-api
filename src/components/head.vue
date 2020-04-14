<template>
    <div id = 'inputs'>
        <input v-model="name" placeholder="name">
        <button v-on:click= 'submit'>Submit</button>
        <app-right :weather = 'info'></app-right>
    </div>
</template>
<script>

import axios from 'axios'
import right from './right'
export default {

    data: ()=> ({
        name: '',
        info: ''
    }),
    components: {
        'app-right': right
    },
    methods:{
    submit: function () {
        axios
        .get(`http://api.openweathermap.org/data/2.5/weather?q=${this.name},us&APPID=764126d68f249066554911a9a05af466`)
        .then(response  => { const data = response.data.main.temp
        let faren = Math.floor(data * 9/5 - 459.67)
        this.info = `${faren} F` 
        })
        }
    }
}    

</script>
<style scoped>

</style>