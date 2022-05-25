<template>
  <div>
    <h1>Hello</h1>
    <p>a :{{ tanga }}</p>
    <p>b : {{ tangb }}</p>
    <button @click="a++">Tang a</button>
    <button @click="b++">Tang b</button>
  </div>
</template>

<script>
// Tat ca du lieu truyen qua html o dang du lieu tho
// computed thuc hien nhu mot function nhung chi duoc coi la 1 t
export default {
  name: "App",
  data() {
    return {
      a: 0,
      b: 0,
    };
  },
  methods: {},
  computed: {
    tanga: function () {
      console.log("tang a");
      return this.a;
    },
    tangb: function () {
      console.log("tang b");
      return this.b;
    },
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
