<template>
<div id="app">
<mt-search
style="height:10%"
  :value.sync="value"
  cancel-text="取消"
  placeholder="请输入昵称，进行约炮">
</mt-search>
<mt-swipe :auto="4000" style="width:367px;height:200px">
  <mt-swipe-item class="s1" name="swipe1Url">1</mt-swipe-item>
  <mt-swipe-item class="s2" name="swipe2Url">2</mt-swipe-item>
  <mt-swipe-item class="s3" name="swipe3Url">3</mt-swipe-item>
</mt-swipe>
</div>
</template>

<script>
import "mint-ui/lib/style.css"
export default {
  name: 'index',
  data () {
    return {
      swipe1Url: '.../assets/images/logo.png./',
      swipe2Url: '../assets/images/swipe1.jpg',
      swipe3Url: '../assets/images/swipe1.jpg',
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
  background-image: url(../assets/images/logo.png);
  background-repeat: no-repeat;
  background-size: 100% 100%;
}
.s1{
  background-image: url(../assets/images/logo.png);
}
/* .s2{
  background-image: url(../assets/images/swipe1.jpg);
}
.s3{
  background-image: url(../assets/images/swipe2.jpg);
} */
.com{
  float: left;
  width: 100%
}
</style>
