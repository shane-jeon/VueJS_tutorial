<!-- Composing with component -->
<template>
  <div class="home">
    <h1>Home Component</h1>
    <Users />
    <Products />
  </div>
</template>

<script>
import Users from "./Users";
import Products from "./Products";

export default {
  // need at least component name
  name: "HomeVue",
  components: {
    Users,
    Products,
  },
};
</script>

<style scoped>
.home {
  background-color: aquamarine;
  height: 500px;
}
</style>

<!-- <template>
  <div> -->
<!-- for loops -->
<!-- <h1>For loop in Vue js</h1>
    <table border="2px">
      <tr>
        <td>Id</td>
        <td>Name</td>
        <td>Email</td>
      </tr>
      <tr v-for="user in users" :key="user.id">
        <td>{{ user.id }}</td>
        <td>{{ user.name }}</td>
        <td>{{ user.email }}</td>
      </tr>
    </table> -->
<!-- conditionals -->
<!-- <h1 v-if="show">Conditional Rendering in Vue js</h1>
    <h1 v-else>else side</h1>
    <button v-on:click="showFunction">toggle</button> -->
<!-- <h1>Hello from Home component</h1> -->
<!-- creating components -->
<!-- <h1>{{ data }}</h1>
    <h1>{{ msg }}</h1>
    <button v-on:click="hello">Call Hello Function</button> -->
<!-- </div> -->
<!-- </template>
<script>
export default {
  name: "HomeVue",
  props: {
    data: String,
    msg: String,
  },
  data() {
    return {
      users: [
        { id: 1, name: "peter", email: "peter@test.com" },
        { id: 2, name: "sammy", email: "sammy@test.com" },
        { id: 3, name: "grace", email: "grace@test.com" },
        { id: 4, name: "richard", email: "dick@test.com" },
      ],
    };
  }, -->
<!-- // data() {
  //   return {
  //     show: false,
  //   };
  // },
  // conditional
  // methods: {
  //   showFunction() {
  //     this.show = !this.show;
  //   },
  // },
  // methods: {
  //   hello(item) {
  //     alert("hello function called", item);
  //   },
  // },
}; -->
<!-- </script> -->
