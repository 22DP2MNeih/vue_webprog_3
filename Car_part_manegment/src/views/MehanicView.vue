<script setup>
import Navbar from '@/components/Navbar.vue'
import PartSearch from '@/components/PartSearch.vue'
</script>

<template>
  <header>
    <Navbar />
  </header>
  <main>
    <PartSearch.vue />
    this is mehanic page
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}
</style>