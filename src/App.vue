<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from '@/components/HelloWorld.vue'
import Navbar from './components/Navbar.vue'
import BackgroundText from './components/BackgroundText.vue'
</script>

<template>

  <header>
    <Navbar />
  </header>
  <BackgroundText ></BackgroundText>
  <RouterView />
</template>

<style>
</style>
