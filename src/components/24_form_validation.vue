<template>
  <h1>22 Simple from</h1>
  <p>{{ from }}</p>
  <ul>
    <li>{{ this.error }}</li>
  </ul>
  <label>Email:</label>
  <input type="text" placeholder="Email" v-model="from.email" />

  <label>Password:</label>
  <input type="password" placeholder="Password" v-model="from.password" />

  <h3>Country:</h3>
  <select v-model="from.country">
    <option>India</option>
    <option>Gujarat</option>
  </select>
  {{ from.email }}
  <h3>Techology:</h3>
  <label>Java :</label>
  <input type="checkbox" value="Java" v-model="from.techo" />
  <label>Javescript :</label>
  <input type="checkbox" value="Javascript" v-model="from.techo" />
  <br />
  <br />

  <h3>Gender</h3>
  <label>Male</label>
  <input type="radio" value="Male" v-model="from.gender" />
  <label>Female</label>
  <input type="radio" value="Female" v-model="from.gender" />
  <br />
  <br />
  <button type="button" v-on:click="getInfo">Submit Data</button>
</template>

<script>
export default {
  name: "simpleForm",
  data() {
    return {
      from: {
        email: "",
        password: "",
        country: "",
        techo: [],
        gender: "",
      },
      error: [],
    };
  },
  methods: {
    getInfo() {
      for (const item in this.from) {
        if (this.from[item] === " " || this.from[item].length === 0) {
          this.error.push(item);
        }
      }
      console.warn("Get information", this.error);
    },
  },
};
</script>
