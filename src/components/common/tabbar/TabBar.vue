<!-- 此处封装的是tabbar的一个整体 -->
<template>
  <div class="tab-bar">
    <slot></slot>
  </div>
</template>

<script>
  export default {
    name: 'TabBar',
    components: {
    }
  }
</script>

<style>
  .tab-bar {
    display: flex;
  }
</style>