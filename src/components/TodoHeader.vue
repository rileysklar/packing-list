<script setup>
import { RouterLink } from "vue-router";
</script>

<template>
  <header>
    <nav class="container">
      <div class="branding">
        <img src="@/assets/Vue_Logo_Black.png" alt="" />
        <h1>Vue.js Packing List</h1>
      </div>
      <ul class="nav-routes">
        <RouterLink :to="{ name: 'todos' }">Home</RouterLink>
        <RouterLink :to="{ name: 'about' }">About</RouterLink>
      </ul>
    </nav>
  </header>
</template>

<style lang="scss" scoped>
header {
  background: rgba(255, 255, 255, 0);
  box-shadow: 0 4px 12px 0 rgba(11, 239, 140, 0.093);
  backdrop-filter: blur(1px);
  -webkit-backdrop-filter: blur(4px);
  border-bottom: 1px solid rgba(255, 255, 255, 0.18);
  nav {
    display: flex;
    align-items: center;
    padding: 25px 16px;

    .branding {
      display: flex;
      align-items: center;
      gap: 8px;
      img {
        max-width: 50px;
      }

      h1 {
        font-size: 24px;
      }

      @media only screen and (max-width: 768px) {
        h1 {
          font-size: 18px;
          margin-right: 30px;
        }
      }
    }

    .nav-routes {
      display: flex;
      flex: 1;
      justify-content: flex-end;
      gap: 12px;
      list-style: none;

      a {
        text-decoration: none;
        color: inherit;
      }

      a:active {
        border-bottom: solid 2px rgb(14, 104, 59);
      }
    }
  }
}
</style>
