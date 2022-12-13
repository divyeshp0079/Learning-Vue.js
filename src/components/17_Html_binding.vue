<template>
  <h1>{{ text }}</h1>
  {{ tag }}
  <div class="htmldata" v-html="tag"></div>
  <div v-html="pass"></div>
</template>

<script>
export default {
  name: "htmlBinding",
  data() {
    return {
      text: "html text",
      tag: "<h1>html add to content</h1>",
      pass: "<h1>html data serve to content</h1>",
    };
  },
};
</script>
