<script setup lang="ts">
import { ref } from 'vue'

const isOpen = ref(false)
function scrollToSection(section: string) {
  const el = document.getElementById(section)
  if (el) {
    el.scrollIntoView({ behavior: 'smooth' })
  }
}
function openMobileNav() {
  isOpen.value = true
}
</script>

<template>
  <nav class="navbar navbar-expand-lg px-3 py-5">
    <div class="grid grid-cols-6">
      <div class="col-span-2"><img src="../assets/Logo.png" style="height: 50px" /></div>

      <div class="hidden md:flex col-span-4 justify-between items-center mr-5">
        <button class="text-xl text-peach" @click="scrollToSection('about')">About</button>
        <button class="text-xl text-peach" @click="scrollToSection('skills')">Skills</button>
        <button class="text-xl text-peach" @click="scrollToSection('projects')">Projects</button>
        <button class="text-xl text-peach" @click="scrollToSection('contact')">Contact</button>
      </div>

      <div class="md:hidden col-span-4 flex justify-end">
        <button @click="openMobileNav" class="texl-xl text-peach">
          <i class="fa-solid fa-bars text-3xl"></i>
        </button>
      </div>
    </div>
    <div
      class="fixed top-0 right-0 w-full h-full bg-studio shadow-lg p-6 text-white transform transition-transform duration-300"
      :class="isOpen ? 'translate-x-0' : 'translate-x-full'"
    >
      <button @click="isOpen = false" class="texl-xl text-peach">
        <i class="fa-solid fa-x text-3xl"></i>
      </button>
    </div>
  </nav>
</template>
