<template>
  <div class="tab">
    <slot></slot>
  </div>
</template>

<script>

export default {
  name: 'TabBar',
}
</script>

<style scoped>
.tab {
  display: flex;
  position: fixed;
  bottom: 0;
  left: 0;
  right: 0;
  border-top: 1px solid #e8e8e8;
  padding-top: 5px;
}
</style>
