<!--  -->
<template>
  <div class='tab-bar-main'>
    <TabBar>
      <TabBarItem path='/home' activeColor='blue'>
        <template v-slot:item-icon>
          <img src="@/assets/img/tabbar/main-uncheck.png" alt="" />
        </template>
        <template v-slot:item-active-icon>
          <img src="@/assets/img/tabbar/main-check.png" alt="" />
        </template>
        <template v-slot:item-text>
          <div>首页</div>
        </template>
      </TabBarItem>
      <TabBarItem path='/category' activeColor='blue'>
        <template v-slot:item-icon>
          <img slot="item-icon" src="@/assets/img/tabbar/cate-uncheck.png" />
        </template>
        <template v-slot:item-active-icon>
          <img slot="item-icon" src="@/assets/img/tabbar/cate-check.png" />
        </template>
        <template v-slot:item-text>
          <div slot="item-text">分类</div>
        </template>
      </TabBarItem>
      <TabBarItem path='/cart' activeColor='blue'>
        <template v-slot:item-icon>
          <img slot="item-icon" src="@/assets/img/tabbar/car-uncheck.png" />
        </template>
        <template v-slot:item-active-icon>
          <img slot="item-icon" src="@/assets/img/tabbar/car-check.png" />
        </template>
        <template v-slot:item-text>
          <div slot="item-text">购物车</div>
        </template>
      </TabBarItem>
      <TabBarItem path='/profile' activeColor='blue'>
        <template v-slot:item-icon>
          <img slot="item-icon" src="@/assets/img/tabbar/mine-uncheck.png" />
        </template>
        <template v-slot:item-active-icon>
          <img slot="item-icon" src="@/assets/img/tabbar/mine-check.png" />
        </template>
        <template v-slot:item-text>
          <div slot="item-text">我的</div>
        </template>
      </TabBarItem>
    </TabBar>
  </div>
</template>

<script>
  import TabBar from '@/components/common/tabbar/TabBar';
  import TabBarItem from '@/components/common/tabbar/TabBarItem';

  export default {
    name: 'TabBarMain',
    components: {
      TabBar,
      TabBarItem
    },
    data() {
      return {

      }
    }
  }
</script>
<style>
  .tab-bar-main {
    position: fixed;
    left: 0;
    right: 0;
    bottom: 0;
  }
</style>