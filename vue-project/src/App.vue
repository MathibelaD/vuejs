<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import NavBar from './components/NavBar.vue'
import Hero from './components/Hero.vue'
import HomeCards from './components/HomeCards.vue'
import GigListing from './components/GigListing.vue'
</script>

<template>
  <NavBar />
  <Hero title="Lets Get to Work" />
  <HomeCards />
  <GigListing :limit="6" />

  <!-- <RouterView /> -->
</template>
