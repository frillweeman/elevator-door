<template>
  <div class="panel">
    <img @click="close" class="button" src="../assets/slice1.svg" alt="">
    <img @click="open" class="button" src="../assets/slice2.svg" alt="">
  </div>
</template>

<script>
import axios from "axios";
export default {
  name: "Panel",
  methods: {
    open() {
      axios.get("/open");
    },
    close() {
      axios.get("/close");
    }
  }
}
</script>

<style scoped>
.panel {
  background-color: #929292;
  margin: 20px 20px;

  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.button {
  height: 200px;
  width: 200px;
  margin-top: 35px;
  margin-bottom: 35px;
}
</style>
