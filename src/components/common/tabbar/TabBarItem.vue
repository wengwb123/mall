<!-- 对tabbar里面的小组件进行封装组合成大组件 -->
<template>
  <div class='tab-bar-item' @click="itemClick">
    <div v-if="!isActive">
      <slot name="item-icon"></slot>
    </div>
    <div v-else>
      <slot name="item-active-icon"></slot>
    </div>
    <div :class="{activeColor: isActive}">
      <slot name="item-text"></slot>
    </div>
  </div>
</template>

<script>

  export default {
    name: 'TabBarItem',
    data() {
      return {
        
      }
    },
    props: {
      path: String,
    },
    computed: {
      isActive() {
        return this.$route.path.indexOf(this.path) !== -1;
      }
    },
    methods: {
      itemClick() {
        this.$router.push(this.path);
      }
    },
  }
</script>

<style>
  .tab-bar-item {
    flex: 1;
    text-align: center;
    height: 49px;
    box-shadow: 0 -1px 1px rgba(100, 100, 100, 0.2);
  }

  .tab-bar-item img {
    width: 24px;
    height: 24px;
    margin-top: 3px;
  }

  .activeColor {
    color: red;
  }
</style>