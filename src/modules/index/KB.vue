<template>
  <div id="app">
    这是index页面的子页面
  </div>
</template>

<script>
import axios from "axios";
export default {
  name: "KB",
  data() {
    return {};
  },
  mounted() {
    axios
      .get("/getJson", {})
      .then(response => {
        console.log(response);
      })
      .catch(error => {
        console.log(error);
      });
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
