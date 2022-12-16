<template>
  <h1>If Else Data</h1>
  <h2 v-if="show">If condition</h2>
  <h2 v-else>Else Data</h2>

  <button v-on:click="show = !show" type="button">Toggle Button</button>
</template>

<script>
export default {
  data() {
    return {
      show: true,
    };
  },
  methods: {
    getValue() {},
  },
};
</script>
