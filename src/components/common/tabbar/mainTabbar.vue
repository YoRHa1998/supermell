<template>
  <div>
    <tab-bar>
      <tab-bar-item path="/home">
      <!-- 给tabbaritem传一个路径值 -->
        <img slot="item-icon" src="~assets/img/tabbar/主页.svg" alt />
        <img slot="item-icon-activated" src="~assets/img/tabbar/主页-activated.svg" alt />
        <div slot="item-text">首页</div>
        <!-- 通过指定插槽名字来具体指定插到哪个插槽中 -->
        <!-- 在tabBar中，将每一个tabBarItem封装成一个组件 -->
      </tab-bar-item>
      <tab-bar-item path="/category">
        <img slot="item-icon" src="~assets/img/tabbar/分类.svg" alt />
        <img slot="item-icon-activated" src="~assets/img/tabbar/分类-activated.svg" alt />
        <div slot="item-text">分类</div>
      </tab-bar-item>
      <tab-bar-item path="/cars">
        <img slot="item-icon" src="~assets/img/tabbar/购物车.svg" alt />
        <img slot="item-icon-activated" src="~assets/img/tabbar/购物车-activated.svg" alt />
        <div slot="item-text">购物车</div>
      </tab-bar-item>
      <tab-bar-item path="/profile">
        <img slot="item-icon" src="~assets/img/tabbar/我的.svg" alt />
        <img slot="item-icon-activated" src="~assets/img/tabbar/我的-activated.svg" alt />
        <div slot="item-text">我的</div>
      </tab-bar-item>
    </tab-bar>
    <!-- 将tabBar封装为一个组件 -->
  </div>
</template>

<script>

import tabBar from "components/common/tabbar/tabBar"; //导入tabBar组件
import tabBarItem from "components/common/tabbar/tabBarItem";

export default {
  components:{
   tabBar, //在components中注册组件
   tabBarItem
  },
  props:{},
  data(){
    return {
    }
  },
  watch:{},
  computed:{},
  methods:{},
  created(){},
  mounted(){}
}
</script>
<style>

</style>