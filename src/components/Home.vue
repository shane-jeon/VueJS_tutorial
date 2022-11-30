<template>
  <div>
    <!-- conditionals -->
    <h1 v-if="show">Conditional Rendering in Vue js</h1>
    <h1 v-else>else side</h1>
    <button v-on:click="showFunction">toggle</button>
    <!-- <h1>Hello from Home component</h1> -->
    <!-- creating components -->
    <!-- <h1>{{ data }}</h1>
    <h1>{{ msg }}</h1>
    <button v-on:click="hello">Call Hello Function</button> -->
  </div>
</template>
<script>
export default {
  name: "HomeVue",
  props: {
    data: String,
    msg: String,
  },
  data() {
    return {
      show: false,
    };
  },
  // conditional
  methods: {
    showFunction() {
      this.show = !this.show;
    },
  },
  // methods: {
  //   hello(item) {
  //     alert("hello function called", item);
  //   },
  // },
};
</script>
