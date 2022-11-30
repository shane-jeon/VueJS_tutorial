<!-- Class and Style Bindings -->
<!-- <template>
  <div>
    <h1 class="vueStyle">Class and Style Bindings</h1>
    Class with Style
    <h1 v-bind:style="{ color: colorName }">Style Bindings</h1>
    <h1 v-bind:class="{ display: show, vueStyle: show }">Class with Object</h1>
    conditional styling
    <h1 v-bind:class="[checkDisplay ? d : v]">Class with Array</h1>
  </div>
</template>

<script>
export default {
  name: "HomeVue",
  data() {
    return {
      colorName: "skyblue",
      show: true,
      // show: false,
      d: "display",
      v: "vueStyle",
      checkDisplay: false,
    };
  },
};
</script> -->

<!-- <style scoped>
.vueStyle {
  color: orange;
}
.display {
  background-color: peru;
  padding: 5px;
}
</style> -->

<!-- templates -->
<template>
  <div>
    <p v-html="header"></p>
    <!-- <h1>Template in vue js</h1> -->
    <!-- 'v-once' only updated once, so on localhost:8081 will display "Shane" but 2nd <h2> will change to "peter" -->
    <h2 v-once>{{ name }}</h2>
    <h2>{{ name }}</h2>
    <button v-bind:disabled="btnDisable" v-on:click="hello">Click me</button>
    <!-- <p>{{ 1 - 100 }}</p> -->
    <h3>{{ ok ? "yes" : "no" }}</h3>
  </div>
</template>

<script>
export default {
  name: "HomeVue",
  // define properties in data method
  data() {
    return {
      name: "Shane",
      ok: true,
      header: "<h1>Template in vue js</h1>",
      btnDisable: true,
    };
  },
  methods: {
    // functions defined here
    hello() {
      // alert("Hello click");
      this.name = "peter";
      // now I can toggle between yes and no
      this.ok = !this.ok;
    },
  },
};
</script>

<!-- Composing with component -->
<!-- <template>
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
</style> -->

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
