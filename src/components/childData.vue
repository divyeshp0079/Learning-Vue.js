<template>
  <h2>{{ name }}</h2>
  <h2>{{ user.name }}</h2>
  <h2>{{ user.email }}</h2>
  <button v-on:click="getData()">Get Function</button>
</template>

<script>
export default {
  name: "childData",
  props: {
    name: String,
    user: Object,
    getData: Function,
  },
};
</script>
