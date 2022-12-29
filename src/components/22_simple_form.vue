<template>
  <h1>22 Simple from</h1>
  <label>Email:</label>
  <input type="text" placeholder="Email" v-model="from.email" />
  {{ from.email }}
  <label>Password:</label>
  <input type="password" placeholder="Password" v-model="from.password" />
  {{ from.password }}
  <button type="button" v-on:click="getInfo">Submit Data</button>
</template>

<script>
export default {
  name: "simpleForm",
  data() {
    return {
      from: {
        email: "",
        password: "",
      },
    };
  },
  methods: {
    getInfo() {
      alert();
      console.warn("Get information", this.from);
    },
  },
};
</script>
