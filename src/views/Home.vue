<script setup lang="ts">
import Nav from '../components/Nav.vue'
</script>

<template>
  <div class="bg-martinique h-screen">
    <div class="max-w-6xl mx-auto px-6 md:px-10">
      <Nav />
      <section id="hero" class="px-8 md:px-20 grid grid-cols-1 md:grid-cols-6 items-center gap-20">
        <div class="col-span-2">
          <img src="../../public/woman.png" alt="Bianca" class="rounded-full shadow-lg" />
        </div>

        <div class="col-span-4 text-right md:text-left">
          <h1 class="text-peach text-5xl md:text-6xl font-bold mb-4">Hi, I'm Bianca</h1>
          <p class="text-pearlstone text-lg md:text-xl max-w-lg">
            Fullstack Web Developer & Online Media Student building interactive, modern websites.
          </p>
        </div>
      </section>
    </div>
  </div>
</template>
