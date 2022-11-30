<template>
  <div>
    <h1>Hello from Home component</h1>
    <h1>{{ data }}</h1>
    <h1>{{ msg }}</h1>
    <button v-on:click="hello">Call Hello Function</button>
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
      show: true,
    };
  },
  // methods: {
  //   hello(item) {
  //     alert("hello function called", item);
  //   },
  // },
};
</script>
