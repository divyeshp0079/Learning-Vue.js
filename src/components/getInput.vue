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
  <childData name="Demo" :user="user" :getData="getData" />
</template>

<script>
import childData from "./childData.vue";
export default {
  name: "getInput",
  components: {
    childData,
  },
  data() {
    return {
      email: " ",
      password: " ",
      demo: " ",
      user: { name: "Divyesh", email: "divyesh@demo.com" },
    };
  },
  methods: {
    getData() {
      alert("demo");
    },
  },
};
</script>
