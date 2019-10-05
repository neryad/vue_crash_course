<template>
  <div id="app">
    {{todos}}
   
  </div>
</template>

<script>


export default {
  name: 'app',
  components: {
    
  },
  data(){
    return{
      todos:[
        {
          id:1,
          title:"Todo One",
          completed:false
        },
        {
           id:2,
          title:"Todo Two",
          completed:false
        },
        {
           id:3,
          title:"Todo three",
          completed:false
        }
      ]
    }
  }
}
</script>

<style>
*{
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body{
  font-family: Arial, Helvetica, sans-serif;
  line-height: 1.4;
}
</style>
