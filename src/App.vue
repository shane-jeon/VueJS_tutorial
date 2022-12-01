<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png" /> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App" /> -->
    <!-- <Home data="Shane is here" msg="we are friends" /> -->
    <!-- <Home /> -->
    <!-- <DataBind /> -->
    <Child v-bind:users="users" />
  </div>
</template>

<script>
// import HelloWorld from "./components/HelloWorld.vue";
// import Home from "./components/Home.vue";
// import Home from "./components/Home";
// import DataBind from "./components/DataBind";
import Child from "./components/Child";
export default {
  name: "App",
  components: {
    // Home,
    // DataBind,
    Child,
  },
  data() {
    return {
      users: [
        { name: "shane", email: "shane@test.com" },
        { name: "anne", email: "anne@test.com" },
        { name: "tom", email: "tom@test.com" },
        { name: "lily", email: "lily@test.com" },
      ],
    };
  },
  // components: {
  //   // HelloWorld,
  //   Home,
  // },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
