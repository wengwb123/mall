<!-- 将上面的导航栏划分为三部分封装成组件 -->
<template>
  <div class='nav-bar'>
    <div class='left'><slot name='left'></slot></div>
    <div class='center'><slot name='center'></slot></div>
    <div class='right'><slot name='right'></slot></div>
  </div>
</template>

<script>

  export default {
    name: 'NavBar',
    components: {},
    data() {
      return {

      }
    }
  }
</script>
<style>
  .nav-bar {
    display: flex;
    line-height: 44px;
    text-align: center;
  }

  .left, .right {
    width: 60px;
  }
  .center {
    flex: 1;
  }
</style>