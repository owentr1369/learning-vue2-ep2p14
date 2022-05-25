<template>
  <div>
    <p>{{ diem }}</p>
    <input type="text" v-model="diem" />
  </div>
</template>

<script>
// Tat ca du lieu truyen qua html o dang du lieu tho
// computed thuc hien nhu mot function nhung chi duoc coi la 1 t
export default {
  name: "App",
  data() {
    return {
      diem: "Ban A co mon toan 7 diem",
    };
  },
  methods: {},
  watch: {
    diem: function () {
      alert("Diem cua ban ay da duoc thay doi sang diem khac");
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
