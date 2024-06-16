<template>
  <div id="app">
    <nav>
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </nav>
    <router-view/>
    <!-- <Footer></Footer> -->
  </div>
</template>
<!-- <script lang="ts">
  import {Footer} from '@/components/HelloWorld.vue';
  import { Options, Vue } from 'vue-class-component';

  // @Options({
  //   components: {
  //     Footer
  //   },
  // })
</script> -->

<style lang="scss">
@import './assets/css/reset.scss';
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
