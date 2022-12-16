<template>
  <h1>My name:{{ getName("Demo") }}</h1>
  <h1>My email:{{ getParaname().email }}</h1>
  <h1>Learning :{{ getParaname().learning }}</h1>
</template>

<script>
export default {
  name: "praticalComponents",
  data() {
    return {
      demo: "vue.js",
    };
  },
  methods: {
    getName(name) {
      return name;
    },
    getParaname() {
      return {
        email: "divyesh@test.com",
        learning: this.demo,
      };
    },
  },
};
</script>
