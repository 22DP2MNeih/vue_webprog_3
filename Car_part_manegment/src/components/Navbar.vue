<script setup>
import { RouterLink, RouterView } from 'vue-router'

</script>

<template>
  <head>
    <link rel="icon" type="image/x-icon" href="../Img/car_parts_logo.avif">
  </head>
  <header>
  <nav>

    <RouterLink to="/">Home</RouterLink>
    <RouterLink to="/about">About</RouterLink>
    <RouterLink to="/login">Login</RouterLink>
    <RouterLink to="/mehanic">Mehanic</RouterLink>
    <RouterLink to="/company">Company</RouterLink>
  </nav>
</header>
  
</template>

<style scoped>

nav {
  width: 100%;
  font-size: 1.5rem;
  text-align: center;
  /* margin-top: 2rem; */
  background-color: rgb(59, 95, 188);
  height: 4rem;
}

header {
  line-height: 1.5;
  max-height: 100vh;
  background-color: rgb(59, 95, 188);
}

a {
  color: whitesmoke;
  margin: 5%;
  margin-bottom: 15%;
  margin-top: 15%;
  text-decoration: none;
}

</style>
