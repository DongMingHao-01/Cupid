<template>
<div id="app">
<mt-swipe :auto="4000" style="width:100%;height:100%">
  <mt-swipe-item>1</mt-swipe-item>
  <mt-swipe-item>2</mt-swipe-item>
  <mt-swipe-item>3</mt-swipe-item>
</mt-swipe>
</div>
</template>

<script>
import "mint-ui/lib/style.css"
export default {
  name: 'index',
  data () {
    return {
      width:''
    }
  },
  methods: {

  },
  mounted: function () {
    this.width =window.screen.width
    console.log(this.width)
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
