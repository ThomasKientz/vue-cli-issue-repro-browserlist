<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    foo : {{ foo.bar }}
    <HelloWorld msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";

const obj = { bar: "baz" };

export default {
  name: "app",
  components: {
    HelloWorld
  },
  data: () => ({
    foo: { ...obj }
  })
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
