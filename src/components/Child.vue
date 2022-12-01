<template>
  <div>
    <h1>Props in Vue js</h1>
    <!-- <h1>Child Component</h1> -->
    <!-- <h3>{{ users }}</h3> -->
    <h3 v-for="user in users" :key="user.name">
      {{ user.name }}
    </h3>
  </div>
</template>

<script>
export default {
  name: "ChildDataBind",
  props: ["users"],
};
</script>
