<template>
  <div class="first">
    <h1>Name : {{ name }}</h1>
    <h1>Email : {{ email }}</h1>
  </div>
  <h1>Surname :{{ getName("Patel") }}</h1>
  <sendChild :getData="getValue" />
</template>

<script>
import sendChild from "./20_send_child_to_parent_data_component.vue";
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
  components: {
    sendChild,
  },
  methods: {
    getValue(userName) {
      alert(userName);
    },
  },
};
</script>

<style>
h1 {
  color: red;
}
</style>
