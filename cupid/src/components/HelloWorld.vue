<template>
<div id="app">
    <mt-button @click.native="handleClick">按钮</mt-button>
  </div>
</template>

<script>
export default {
  name: 'index',
  data () {
    return {
    }
  },
  methods: {
    handleClick: function(){
      alert(666)
    }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#app {
background-color: #000;
margin-top: 0;
}
</style>
