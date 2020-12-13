<template>
  <div>
    <router-view></router-view>
    <TabBarMain/>
  </div>
</template>

<script>
  import TabBarMain from '@/components/content/tabbarcontent/TabBarMain.vue';

  export default {
    name: 'App',
    components: {
      TabBarMain
    }
  }

</script>

<style>
  @import 'assets/css/base.css';
</style>