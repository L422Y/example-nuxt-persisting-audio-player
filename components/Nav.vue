<template>
  <nav>
    <NuxtLink to="/">Home</NuxtLink>
    <NuxtLink to="/music">Music</NuxtLink>
    <NuxtLink to="/music/techno">Music: Techno</NuxtLink>
    <NuxtLink to="/music/progressive-house">Music: Progressive House</NuxtLink>
  </nav>
</template>
<style scoped>
nav {
  display: flex;
  gap: 1rem;
  margin: 1rem 0;
}
a.router-link-active {
  font-weight: bold;
}
</style>
