<template>
<div id="app">
    <mt-button type="default">default</mt-button>
        <mt-button type="primary">primary</mt-button>
        <mt-button type="danger" >danger</mt-button>
    <router-view/>
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
    // handleClick: function(){
    //   alert(666)
    // }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#app{
  width: 100%;
  height: 100%;
  background-color: #000;
}
.com{
  float: left;
  width: 100%
}
</style>
