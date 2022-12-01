<template>
  <div>
    <button v-on:click="updateTitle">Update Title</button>
  </div>
</template>

<script>
export default {
  name: "ChildComponent",
  methods: {
    updateTitle() {
      // console.warn("updateTitle");
      // emit takes 2 parameters: 1. event name, 2. Your chosen title
      this.$emit("changeTitle", "Props have been passed");
    },
  },
};
</script>
