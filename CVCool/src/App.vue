<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <header>
    <img alt="profile_pic" class="logo" src="@/assets/pp.png"  width="250" />

    <div class="wrapper">
      <HelloWorld msg="Brandon Estefan Núñez Maturana" />

      <nav>
        <RouterLink to="/">Professional</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style scoped>

.logo {
  display: flex;
  margin: 0 3rem 1rem 1rem;
  border-radius: 1rem;
  padding-left: 0%;
  size: 100%;
}
nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
  
}
nav a.router-link-exact-active {
  color:rgb(197, 127, 255);
}
nav a.router-link-exact-active:hover {
  background-color: transparent;
}
nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}
nav a:first-of-type {
  border: 0;
}
@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }
  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;
    padding: 1rem 0;
    margin-top: 1rem;
  }
  header {
  line-height: 1.5;
  max-height: 100vh;
  }
}
</style>