<template>
  <h1>Forloop</h1>
  <ul>
    <li v-for="item in techonlogy" :key="item">
      {{ item }}
    </li>
  </ul>
  <ul>
    <li v-for="developer in user" :key="developer">
      Name is a {{ developer.name }} and email {{ developer.email }}
    </li>
  </ul>
  <br />
  <br />
  <br />
</template>

<script>
export default {
  data() {
    return {
      techonlogy: ["shopify", "bigcommerce", 2022, "wordpress"],
      user: [
        { name: "Divyesh", email: "divyeshpatel081996@gmail.com" },
        { name: "demo", email: "divyeshpatel081996@gmail.com" },
        { name: "test", email: "divyeshpatel081996@gmail.com" },
      ],
    };
  },
};
</script>
