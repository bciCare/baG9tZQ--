// TODO: nav foot type shi

<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <nav>
    <RouterLink to="/login">Login</RouterLink>
  </nav>

  <RouterView />

  <footer>
    <div id="copyright">
      <p>bCore, Copyright &copy; 2024</p>
    </div>
    <div id="socials">
      <div id="github">
        <a href="https://github.com/blazi06">
          <img
            src="https://github.githubassets.com/assets/GitHub-Mark-ea2971cee799.png"
            height="20px"
            width="20px"
          />
        </a>
      </div>
    </div>
    <div id="contact">
      <a href="mailto:blaz@bcore.tech">Contact</a>
    </div>
  </footer>
</template>

<style scoped>
nav {
  display: flex;
  align-items: center;
  justify-content: right;
  padding: 5px 15px;
  border-bottom: rgb(97, 97, 97) 1px dashed;
}

nav a {
  color: rgb(136, 136, 136);
  text-decoration: none;
  padding: 2px 10px 2px 10px;
  background: black;
}

footer {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 5px 15px;
}

#copyright {
  width: 30%;
}

#contact {
  text-align: right;
  width: 30%;
}
</style>
