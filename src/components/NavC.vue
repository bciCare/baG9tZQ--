<script setup>
import { RouterLink } from 'vue-router'
</script>

<template>
  <nav class="bordered-component">
    <div id="return">
      <RouterLink v-if="$route.name !== 'home'" class="routerlink" to="/"
        >Home</RouterLink
      >
    </div>
    <div id="socialsnlinks">
      <div id="github">
        <a href="https://github.com/blazi06/baG9tZQ--">
          <img
            height="25"
            id="svg_github"
            src="@/assets/images/github.svg"
            alt="github logo"
            width="25"
          />
        </a>
      </div>
      <RouterLink class="routerlink" to="/login">Login</RouterLink>
    </div>
  </nav>
</template>

<style scoped>
@import '@/assets/styles/scoped/NavC.css';
</style>
