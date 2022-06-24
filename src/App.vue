<template>
  <div id="app">
    <panel />
  </div>
</template>

<script>
import Panel from "./components/Panel.vue";

export default {
  name: 'App',
  components: {
    Panel
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

body {
  margin: 0;
  background-color: #656565;
}
</style>
