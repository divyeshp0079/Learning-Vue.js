<template>
  <div class="user">
    <h2>{{ data.name }}</h2>
    <h2>{{ data.email }}</h2>
    <button v-on:click="getValue(data.name)">Alert message</button>
  </div>
</template>

<script>
export default {
  name: "reuseComponent",
  props: {
    data: Object,
    getValue: Function,
  },
};
</script>
