<script setup lang="ts">
const stars = Array.from({ length: 150 }, () => ({
  top: Math.random() * 200,
  left: Math.random() * 100,
  size: Math.random() * 3 + 1,
  duration: Math.random() * 200 + 100,
}))
</script>

<template>
  <div class="absolute inset-0 overflow-hidden">
    <div
      v-for="(star, i) in stars"
      :key="i"
      class="absolute bg-white rounded-full animate-[floatStars_linear_infinite]"
      :style="{
        top: star.top + '%',
        left: star.left + '%',
        width: star.size + 'px',
        height: star.size + 'px',
        animationDuration: star.duration + 's',
      }"
    ></div>
  </div>
</template>
