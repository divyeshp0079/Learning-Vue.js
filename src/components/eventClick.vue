<template>
  <h1 v-on:mouseover="getValue()">{{ mouseover }}</h1>
  <button v-on:click="getData()">{{ count }}</button>
  <button v-on:dblclick="getPrice('1996')">{{ price }}</button>
  <h1>{{ number }}</h1>
  <input type="text" v-model="data" />
  <h1>{{ data }}</h1>
</template>

<script>
export default {
  name: "clickEvent",
  data() {
    return {
      name: "divyesh",
      price: "price",
      mouseover: "Mouse over show value",
      count: "count",
      number: 0,
      data: 10,
    };
  },
  methods: {
    getData() {
      this.number = this.number + 1;
    },
    getPrice() {
      this.number = this.number - 1;
    },
    getValue() {
      console.log("Show the value");
    },
  },
};
</script>
