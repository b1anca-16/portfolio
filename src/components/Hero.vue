<script setup lang="ts">
import { ref } from 'vue'
</script>

<template>
  <section id="hero" class="grid grid-cols-1 lg:grid-cols-5 items-center gap-20">
    <div class="lg:col-span-2 flex justify-center item-center">
      <img src="../../public/woman.png" alt="Bianca" class="rounded-full bg-studio max-h-100" />
    </div>
    <div class="lg:col-span-3">
      <h1 class="text-peach font-caveat text-4xl font-bold mb-4">Hi, I'm Bianca</h1>
      <div class="text-peach text-5xl md:text-6xl font-bold leading-tight">
        An Online Media student building <span class="text-outline-peach">fullstack</span> web
        experiences.
      </div>
    </div>
  </section>
</template>
