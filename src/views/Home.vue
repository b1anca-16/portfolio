<script setup lang="ts">
import Nav from '../components/Nav.vue'
import Hero from '../components/Hero.vue'
import StarBackground from '../components/StarBackground.vue'
</script>

<template>
  <div class="bg-martinique min-h-screen relative overflow-hidden">
    <StarBackground />
    <div class="relative z-10 max-w-6xl mx-auto px-6 md:px-10">
      <Nav />
      <div class="h-[calc(100vh-80px)] flex items-center">
        <Hero />
      </div>
    </div>
  </div>
</template>
