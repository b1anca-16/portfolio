<script setup lang="ts">
import Nav from '../components/Nav.vue'
import Hero from '../components/Hero.vue'
</script>

<template>
  <div class="bg-martinique h-screen">
    <div class="max-w-6xl mx-auto px-6 md:px-10">
      <Nav />
      <div class="h-[calc(100vh-80px)] flex-1 flex items-center">
        <Hero />
      </div>
    </div>
  </div>
</template>
