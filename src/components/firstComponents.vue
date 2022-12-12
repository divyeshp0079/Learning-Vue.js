<template>
  <div class="first">
    <h1>Name : {{ name }}</h1>
    <h1>Email : {{ email }}</h1>
  </div>
  <h1>Surname :{{ getName("Patel") }}</h1>
</template>

<script>
export default {
  name: "firstComponents",
  data() {
    return {
      name: "Divyesh",
      email: "divyesh.patel081996@gmail.com",
      getName: function (a) {
        return a;
      },
    };
  },
};
</script>

<style>
h1 {
  color: red;
}
</style>
