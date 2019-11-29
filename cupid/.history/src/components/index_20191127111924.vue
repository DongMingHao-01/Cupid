<template>
<div id="app">
<mt-search
  :value.sync="value"
  cancel-text="取消"
  placeholder="请输入昵称，进行约炮">
</mt-search>
<mt-swipe :auto="4000" style="width:367px;height:200px">
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
  background-image: url(../assets/logo.png);
  background-repeat: no-repeat;
  background-size: 100% 100%;
}
.com{
  float: left;
  width: 100%
}
</style>
