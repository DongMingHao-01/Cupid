<template>
<div id="app">
<mt-search
style="height:10%"
  :value.sync="value"
  cancel-text="取消"
  placeholder="请输入昵称，进行搜索">
</mt-search>
<mt-swipe :auto="4000" style="width:360px;height:100px">
  <mt-swipe-item class="s1"></mt-swipe-item>
  <mt-swipe-item class="s2"></mt-swipe-item>
  <mt-swipe-item class="s3"></mt-swipe-item>
</mt-swipe>
<!-- <ul class="tag">
  <li v-for="(item, index) in items">{{item.message}}</li>
</ul> -->
<mt-badge type="primary" size="small" style="margin-left:10px" v-for="item in items" v-bind:key="item.id">{{item.message}}</mt-badge>
</div>
</template>

<script>
import "mint-ui/lib/style.css"
export default {
  name: 'index',
  data () {
    return {
      items:[
        {message:'颜控'},
        {message:'可爱风'},
        {message:'萝莉'},
        {message:'90后'},
        {message:'程序员'},
        {message:'头发多'},

      ],
      width:'',
      height: ''
    }
  },
  methods: {

  },
  mounted: function () {
    this.width =window.screen.width
    this.height =window.screen.height
    console.log(this.width)
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#app{
  background-image: url(../assets/images/bgc.jpg);
  background-repeat: no-repeat;
  background-size: 100% 100%;
}
.s1{
  background-image: url(../assets/images/logo.png);
}
 .s2{
  background-image: url(../assets/images/swipe1.jpg);
}
.s3{
  background-image: url(../assets/images/swipe2.png);
}
.com{
  float: left;
  width: 100%
}
</style>
