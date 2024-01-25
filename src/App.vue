<script setup>
import { RouterView } from "vue-router";
import TodoHeader from "./components/TodoHeader.vue";
</script>

<template>
  <TodoHeader />
  <RouterView />
</template>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Source+Code+Pro:ital,wght@0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap");

* {
  font-family: "Source Code Pro", sans-serif;
  margin: 0;
  padding: 0;
  letter-spacing: -1px;
  box-sizing: border-box;
  color: #fafafa;
}
.container {
  max-width: 1100px;
  margin: 0 auto;
}
body {
  background-image: url("@/assets/topo.png");
  background-size: cover;
  background-repeat: no-repeat;
  min-height: 100svh;
}
</style>
