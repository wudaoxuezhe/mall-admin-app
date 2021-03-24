<template>
  <div class="home">
    <left-menu></left-menu>
    <div class="main-app" :class="{ 'menu-fold': $store.state.collapsed }">
      <header-info></header-info>
      <router-view></router-view>
    </div>
  </div>
</template>

<script>
import LeftMenu from './components/menu.vue';
import HeaderInfo from './components/header.vue';

export default {
  data() {
    return {
    };
  },
  components: {
    LeftMenu,
    HeaderInfo,
  },
  methods: {
  },
};
</script>

<style lang="less">
// 把@当做模块编译成src目录，前面要加~
@import url("~@/assets/css/home.less");
</style>
