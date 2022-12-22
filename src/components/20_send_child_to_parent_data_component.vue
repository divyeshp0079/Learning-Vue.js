<template>
  <h1>Child Data</h1>
  <button v-on:click="getData(userName)">Get user name</button>
</template>

<script>
export default {
  data() {
    return {
      userName: "peter",
    };
  },
  props: {
    getData: Function,
  },
};
</script>
