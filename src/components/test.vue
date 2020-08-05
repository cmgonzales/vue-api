<template>
    <div id = 'test'>
        <p v-if = "see"> test</p>
        <p><button v-on:click = "see = !see">this is a sumbit</button></P>

        </div>
</template>
<script>

export default {
    el: '#test',
    data: () => ({
        see: false,
  
      
    })
    
}
</script>