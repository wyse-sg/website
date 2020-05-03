<template>
  <div class="main-content">
    <div class="main-content--body">
      <div class="left">
        <List/>
      </div>
      <div class="right">
        <router-view/>
      </div>
    </div>
    <Header/>
  </div>
</template>

<script>

import Header from './Header.vue';
import List from './List.vue';

export default {
  name: 'Main',
  components: {
    Header,
    List,
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
        // flex-grow: 1;
        height: 40%;
        border-right: 1px solid #bbb;
        padding: 0 5%;
      }

      .right {
        width: 50%;
        height: 40%;
        display: flex;
        flex-direction: column;
        justify-content: center;
        padding: 0 5%;
        text-align: left;
      }
    }
  }
</style>
