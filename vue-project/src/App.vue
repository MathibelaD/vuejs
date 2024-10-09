<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import NavBar from './components/NavBar.vue'
import Hero from './components/Hero.vue'
import HomeCards from './components/HomeCards.vue'
</script>

<template>
  <NavBar />
  <Hero title="Lets Get to Work" />
  <HomeCards />

  <!-- <RouterView /> -->
</template>
