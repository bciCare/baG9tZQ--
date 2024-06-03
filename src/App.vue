// TODO: nav foot type shi

<script setup>
import { RouterLink, RouterView } from 'vue-router'
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
            width="25"
          />
        </a>
      </div>
      <RouterLink class="routerlink" to="/login">Login</RouterLink>
    </div>
  </nav>

  <RouterView />

  <footer class="bordered-component">
    <div id="copyright">
      <p>&copy; 2024 bcore</p>
    </div>
    <div id="contact">
      <a class="routerlink" href="mailto:blaz@bcore.tech">Contact</a>
    </div>
  </footer>
</template>

<style scoped>
nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin: 8px 12px;
  padding: 1px 2px;
  height: 35px;
}

#socialsnlinks {
  display: flex;
  gap: 10px;
}

#socialsnlinks > div {
  display: flex;
  align-items: center;
  justify-content: center;
}

#socialsnlinks > div > a {
  height: 25px;
}

.routerlink {
  color: var(--color-text);
  text-decoration: none;
  padding: 2px 10px 2px 10px;
}

footer {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 35px;
  margin: 8px 12px;
  padding: 1px 2px;
}

footer > div {
  width: 30%;
}

#contact {
  text-align: right;
}
</style>
