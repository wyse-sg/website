<template>
  <div class="main-content">
    <div class="main-content--body">
      <div class="left">

      </div>
      <div class="right">

      </div>
    </div>
    <Header/>
  </div>
</template>

<script>

import Header from './Header.vue';

export default {
  name: 'Main',
  components: {
    Header,
  },
};
</script>

<style scoped lang="scss">
  .main-content {
    height: 100vh;
    display: flex;
    flex-direction: column;

    .main-content--body {
      position: absolute;
      display: flex;
      flex-direction: row;
      justify-content: center;
      align-items: center;
      height: 100vh;
      width: 100%;

      .left {
        width: 50%;
        height: 40%;
        border-right: 1px solid #bbb;
      }
      .right {
        width: 50%;
        height: 40%;
      }
    }
  }
</style>
