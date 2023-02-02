<template>
  <h1>Modifiers From Modifiers</h1>
  <input type="text" v-model.number.lazy.trim="email" />
  <input v-model.number="phone" />
  {{ email }}
  {{ phone }}
</template>

<script>
export default {
  data() {
    return {
      email: "",
      phone: "",
    };
  },
};
</script>
