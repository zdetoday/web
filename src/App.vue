<template>
  <router-view />
  <Footer />
</template>
<script lang="ts">
// import Vue from "vue";
// import { Options } from "vue-class-component";
import { Options, Vue } from "vue-class-component";
import Footer from "./components/BottomFooter.vue"; // @ is an alias to /src

@Options({
  components: {
    Footer,
  },
})
export default class App extends Vue {}
</script>

<style lang="less">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  // text-align: center;
  color: #2c3e50;
}

#nav {
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
