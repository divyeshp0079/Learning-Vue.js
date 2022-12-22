<template>
  <h1>Ref with interview question</h1>
  <input type="text" ref="data" />
  <button v-on:click="getValue">Get value data</button>
</template>

<script>
export default {
  name: "HomeData",
  methods: {
    getValue() {
      this.$refs.data.focus();
      let val = this.$refs.data.value;
      this.$refs.data.style.color = "blue";
      console.warn(val);
    },
  },
};
</script>
