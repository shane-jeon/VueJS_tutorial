<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png" /> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App" /> -->
    <!-- <Home data="Shane is here" msg="we are friends" /> -->
    <!-- <Home /> -->
    <!-- <DataBind /> -->
    <!-- <Child v-bind:users="users" /> -->
    <Child2 v-on:changeTitle="updateTitleText($event)" />
    <h1>{{ title }}</h1>
  </div>
</template>

<script>
// import HelloWorld from "./components/HelloWorld.vue";
// import Home from "./components/Home.vue";
// import Home from "./components/Home";
// import DataBind from "./components/DataBind";
// import Child from "./components/Child";
import Child2 from "./components/Child2";
export default {
  name: "App",
  components: {
    // Home,
    // DataBind,
    // Child,
    Child2,
  },
  data() {
    return {
      title: "Child to Parent Data",
    };
  },
  methods: {
    updateTitleText(title) {
      this.title = title;
    },
  },
  // data() {
  //   return {
  //     users: [
  //       { name: "shane", email: "shane@test.com" },
  //       { name: "anne", email: "anne@test.com" },
  //       { name: "tom", email: "tom@test.com" },
  //       { name: "lily", email: "lily@test.com" },
  //     ],
  //   };
  // },
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
