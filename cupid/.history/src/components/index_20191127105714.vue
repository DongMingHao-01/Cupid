<template>
<div id="app">

</div>
</template>

<script>
import "mint-ui/lib/style.css"
export default {
  name: 'index',
  data () {
    return {
      width:'',
      height: ''
    }
  },
  methods: {

  },
  mounted: function () {
    this.width =window.screen.width
    this.height =window.screen.height

    console.log(this.height)
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#app{

}
.com{
  float: left;
  width: 100%
}
</style>
