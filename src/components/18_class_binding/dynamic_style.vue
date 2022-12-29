<template>
  <h1 :class="applyStyle">Home component</h1>
  <button v-on:click="colorfull = !colorfull">Change color</button>
</template>

<script>
export default {
  name: "dyamicStyle",
  data() {
    return {
      colorfull: true,
    };
  },
  computed: {
    applyStyle() {
      return {
        green: this.colorfull,
        err: true,
        other: true,
      };
    },
  },
};
</script>

<style>
.green {
  background-color: green;
  width: 400px;
  padding: 10px;
  margin: 0 auto;
}

.err {
  color: red;
}

.other {
  font-size: 50px;
}
</style>
