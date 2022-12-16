<template>
  <h1>Get Check Box & Radio Button</h1>
  <br />
  <br />
  <h3>Technology</h3>
  <label for="shopify">Shopify</label>
  <input type="checkbox" value="shopify" v-model="technology" id="shopify" />
  <br />
  <br />
  <label for="php">php</label>
  <input type="checkbox" value="php" v-model="technology" id="php" />
  <br />
  <br />
  <h3>Who I am</h3>

  <label for="developer">Developer</label>
  <input type="radio" value="developer" v-model="who" id="developer" />

  <label for="student">Student</label>
  <input type="radio" value="student" v-model="who" id="checkbox" />

  <h2>Select Technology : {{ technology }}</h2>
  <h2>I am a:{{ who }}</h2>
</template>

<script>
export default {
  name: "getCheck",
  data() {
    return {
      technology: [],
      who: [],
    };
  },
};
</script>
