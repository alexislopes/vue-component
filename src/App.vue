<template>
  <div id="app">
    <input-numbers @sendOne="one = $event" @sendTwo="two = $event"></input-numbers>
    <exec-numbers :one="this.one" :two="this.two"></exec-numbers>
  </div>
</template>

<script>
import InputNumbers from "./components/InputNumbers.vue";
import ExecNumbers from "./components/ExecNumbers.vue";

export default {
  name: "app",

  data() {
    return {
      one: 0,
      two: 0
    };
  },
  components: {
    "input-numbers": InputNumbers,
    "exec-numbers": ExecNumbers
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
