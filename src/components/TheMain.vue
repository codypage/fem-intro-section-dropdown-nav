<script setup>
import { defineAsyncComponent } from 'vue'
const TheHero = defineAsyncComponent(() => import('./TheHero.vue'))
</script>

<template>
  <main>
    <TheHero />
  </main>
</template>

<style lang="scss"></style>
