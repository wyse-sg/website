<template>
  <div id="app">
    <Jumbotron/>
    <Main/>
    <!-- <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>
    <router-view/> -->
  </div>
</template>

<script>
// // @ is an alias to /src
import Jumbotron from '@/components/Jumbotron.vue';
import Main from '@/components/Main.vue';

export default {
  name: 'App',
  components: {
    Jumbotron,
    Main,
  },
};

</script>

<style lang="scss">
  body {
    margin: 0px;
  }

  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;

    .px-0.1 {
      padding: 0 10%;
    }
  }
</style>
