<template>
  <!-- <firstComponents></firstComponents>
  <praticalComponents></praticalComponents>
  <eventClick></eventClick>
  <getInput></getInput> -->
  <getcheckbox></getcheckbox>
</template>

<script>
// import firstComponents from "./components/firstComponents.vue";
// import praticalComponents from "./components/praticalComponents.vue";
// import eventClick from "./components/eventClick.vue";
// import getInput from "./components/getInput.vue";
import getcheckbox from "./components/GetCheckbox&RadioButtonValue.vue";
export default {
  name: "App",
  components: {
    // firstComponents,
    // praticalComponents,
    // eventClick,
    // getInput,
    getcheckbox,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
