<script setup>
import {RouterLink, RouterView} from 'vue-router'
</script>

<template>
  <header>
    <div class="wrapper">
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
        <RouterLink to="/login">Login</RouterLink>
      </nav>
    </div>
  </header>
  <RouterView/>
</template>

<style scoped>
header {
  height: 20%;
  width: 100%;
  position: fixed;
  top: 0;
  left: 0;
  z-index: 999;
}

nav {
  width: 100%;
  font-size: 20px;
  text-align: left;
  margin-top: 2rem;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}
</style>
