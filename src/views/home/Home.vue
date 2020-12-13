<!--  -->
<template>
  <div class='home'>
    <NavBar>
      <template v-slot:center>
        购物街
      </template>
    </NavBar>
  </div>
</template>

<script>
  import NavBar from '@/components/common/navbar/NavBar';

  export default {
    name: 'Home',
    components: {
      NavBar,
    },
    data() {
      return {

      }
    }
  }
</script>
<style>
  .home {
    background-color: pink;
    color: #fff;
  }
</style>