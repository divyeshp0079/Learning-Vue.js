<template>
  <br />
  <input type="text" v-model="email" />
  <br />
  <br />
  <input type="password" v-model="password" />
  <br />
  <br />
  <!-- start Two-way binding -->
  <input type="text" v-model="demo" />
  <br />
  <br />
  <h1>{{ demo }}</h1>
  <!-- End Two-way binding -->
  <button type="button" v-on:click="getValue()">Submit</button>
</template>

<script>
export default {
  name: "getInput",
  data() {
    return {
      email: " ",
      password: " ",
      demo: " ",
    };
  },
  methods: {
    getValue() {
      console.warn("values: ", this.email, this.password);
    },
  },
};
</script>
