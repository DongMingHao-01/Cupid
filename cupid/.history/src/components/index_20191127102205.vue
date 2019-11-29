<template>

<mt-swipe :auto="4000">
  <mt-swipe-item name = "one">1</mt-swipe-item>
  <mt-swipe-item name = "two">2</mt-swipe-item>
  <mt-swipe-item name = "three">3</mt-swipe-item>
</mt-swipe>

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
