<template>
  <div id="app">
    <router-view />
    <main-tab-bar></main-tab-bar>
  </div>
</template>

<script>
import MainTabBar from 'components/content/mainTabBar/MainTabBar.vue';

export default {
  components: {
    MainTabBar
  }
}
</script>

<style lang="less">
* {
  margin: 0;
  padding: 0;
}
</style>
