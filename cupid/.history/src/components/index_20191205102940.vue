<template>
<div id="app" :style="  {height: scrollerHeight}">
<mt-search
style="height:10%"
  :value.sync="value"
  cancel-text="取消"
  placeholder="请输入昵称，开始搜索">
</mt-search>
<mt-swipe :auto="4000" style="width:360px;height:90px">
  <mt-swipe-item class="s1"></mt-swipe-item>
  <mt-swipe-item class="s2"></mt-swipe-item>
  <!-- <mt-swipe-item class="s3"></mt-swipe-item> -->
</mt-swipe>
<mt-badge type = "primary" size = "small" style = "margin:70px 10px 30px 0" v-for = "item in items" v-bind:key = "item.id">{{item.message}}</mt-badge>
<img :src = "contentUrl" alt="" @click="fn">
<mt-tabbar :selected.sync="selected">
  <mt-tab-item id = "外卖">
    <img slot = "icon" >
    倾心
  </mt-tab-item>
  <mt-tab-item id = "订单">
    <img slot = "icon" >
    广场
  </mt-tab-item>
  <mt-tab-item id = "发现">
    <img slot = "icon" >
    发布
  </mt-tab-item>
  <mt-tab-item id = "我的">
    <img slot = "icon" >
    聊天
  </mt-tab-item>
  <mt-tab-item id = "我的">
    <img slot = "icon" >
    我的
  </mt-tab-item>
</mt-tabbar>
</div>
</template>

<script>

// import "mint-ui/lib/style.css"
export default {
  name: 'index',
  data () {
    return {
      // contentUrl: require('../assets/images/index.jpg'),
      value:'',
      selected: '',
      items:[
        {message:'颜控'},
        {message:'可爱风'},
        {message:'萝莉'},
        {message:'90后'},
        {message:'程序员'},
        {message:'头发多'},

      ],

    }
  },
  methods: {
    fn : function(){
      console.log(111)
    },
  },
  mounted: function () {
    console.log(666)
  },
  computed: {
    // 滚动区高度
    // (业务需求：手机屏幕高度减去头部标题和底部tabbar的高度，当然这2个高度也是可以动态获取的)
    scrollerHeight: function() {
      return (window.innerHeight - 46 - 50) + 'px';
    }
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#app{
  background-image: url(../assets/images/index.jpg);
  background-repeat: no-repeat;
  background-size: 100% 100%;
}
.s1{
  background-image: url(../assets/images/swipe1.png);
  background-size: contain;
}
 .s2{
  background-image: url(../assets/images/swipe2.png);
  background-size: contain;
}
/* .s3{
  background-image: url(../assets/images/swipe2.png);
} */
.com{
  float: left;
  width: 100%
}
</style>
