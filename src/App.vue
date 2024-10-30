<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    <div class="wrapper">
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header>
  <RouterView />
</template>

<style scoped>
header {
  display: flex;
  align-items: center;
  justify-content: left;
  height: 80px;
  padding: 0 2rem;
  width: 100vw;
  position: fixed;
  z-index: 1000;
}

nav {
  display: flex;
  align-items: center;
  gap: 3rem;
  z-index: 100006;
}

nav a {
  font-weight: 700;
  font-size: 1.3rem;
}
</style>
