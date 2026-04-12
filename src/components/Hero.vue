<script setup lang="ts">
import { ref } from 'vue'
</script>

<template>
  <section id="hero" class="grid grid-cols-1 md:grid-cols-6 items-center gap-20">
    <div class="md:col-span-2 flex justify-center md:justify-start">
      <img src="../../public/woman.png" alt="Bianca" class="rounded-full shadow-lg" />
    </div>
    <div class="md:col-span-4">
      <h1 class="text-peach font-caveat text-4xl font-bold mb-4">Hi, I'm Bianca</h1>
      <div class="text-peach text-6xl leading-20 font-bold">
        A <span class="text-outline-peach">Fullstack</span> Web Developer and Online Media student
        passionate about building <span class="text-outline-peach">interactive experiences</span>.
      </div>
    </div>
  </section>
</template>
