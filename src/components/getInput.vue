<template>
  <!-- <br />
  <input type="text" v-model="email" />
  <br />
  <br />
  <input type="password" v-model="password" />
  <br />
  <br /> -->
  <!-- start Two-way binding -->
  <!-- <input type="text" v-model="demo" /> -->
  <!-- <br />
  <br />
  <h1>{{ demo }}</h1> -->
  <!-- End Two-way binding -->
  <!-- <button type="button" v-on:click="getValue()">Submit</button> -->
  <!-- <childData name="Demo" :user="user" :getData="getData" /> -->
  <ul>
    <li v-for="user in userData" :key="user.name">
      <!-- {{ user }} -->
      <reuseComponent :data="user" :getValue="getValue" />
    </li>
  </ul>
</template>

<script>
// import childData from "./childData.vue";
import reuseComponent from "./16_Reuse_component.vue";
export default {
  name: "getInput",
  components: {
    // childData,
    reuseComponent,
  },
  data() {
    return {
      // email: " ",
      // password: " ",
      // demo: " ",
      userData: [
        {
          name: "data",
          email: "data@test.com",
        },
        {
          name: "test",
          email: "test@data.com",
        },
      ],
    };
  },
  methods: {
    getData() {
      alert("demo");
    },
    getValue(name) {
      alert(name);
    },
  },
};
</script>

<style>
.user {
  background-color: aqua;
  border-bottom: 1px solid #000;
  padding: 10px;
  margin: 20px;
  text-align: left;
}
</style>
