<template>
  <tab-bar>
    <tab-bar-item path="/home">
      <img slot="img"
           src="../../../assets/img/tabbar/home.svg"
           alt="">
      <img slot="activeImg"
           src="../../../assets/img/tabbar/home_active.svg"
           alt="">
      <div slot="itemTitle">首页</div>
    </tab-bar-item>
    <tab-bar-item path="/category">
      <img slot="img"
           src="../../../assets/img/tabbar/category.svg"
           alt="">
      <img slot="activeImg"
           src="../../../assets/img/tabbar/category_active.svg"
           alt="">
      <div slot="itemTitle">分类</div>
    </tab-bar-item>
    <tab-bar-item path="/shopcart">
      <img slot="img"
           src="../../../assets/img/tabbar/shopcart.svg"
           alt="">
      <img slot="activeImg"
           src="../../../assets/img/tabbar/shopcart_active.svg"
           alt="">
      <div slot="itemTitle">购物车</div>
    </tab-bar-item>
    <tab-bar-item path="/profile">
      <img slot="img"
           src="../../../assets/img/tabbar/profile.svg"
           alt="">
      <img slot="activeImg"
           src="../../../assets/img/tabbar/profile_active.svg"
           alt="">
      <div slot="itemTitle">个人</div>
    </tab-bar-item>
  </tab-bar>
</template>

<script>
import TabBar from '../../common/tabbar/TabBar';
import TabBarItem from '../../common/tabbar/TabBarItem';

export default {
  components: {
    TabBar,
    TabBarItem
  }
}
</script>

<style>
</style>
