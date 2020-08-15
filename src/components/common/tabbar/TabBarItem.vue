<template>
  <div class="tabItem"
       @click="itemClick">
    <div v-if="active">
      <slot name="img"></slot>
    </div>
    <div v-else>
      <slot name="activeImg"></slot>
    </div>
    <div :style="activeStyle">
      <slot name="itemTitle"></slot>
    </div>
  </div>
</template>

<script>
export default {
  name: 'TabBarItem',
  methods: {
    itemClick() {
      console.log(this.path);
      this.$router.replace(this.path)
    }
  },
  // data数据
  data() {
    return {
    }
  },
  props: {
    path: String,
    activeColor: {
      type: String,
      default: 'red'
    }
  },
  computed: {
    active() {
      return this.$route.path.indexOf(this.path) === -1
    },
    activeStyle() {
      return this.active ? '' : { color: this.activeColor }
    }
  }
}
</script>

<style lang="less" scoped>
.tabItem {
  flex: 1;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-evenly;
  height: 49px;
  img {
    width: 20px;
    height: 20px;
  }
}
.activeClass {
  color: pink;
}
</style>
