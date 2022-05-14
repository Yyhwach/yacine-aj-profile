<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from '@/components/HelloWorld.vue'
import Navbar from './components/Navbar.vue'
import BackgroundText from './components/BackgroundText.vue'
</script>

<template>
  <div id="cristiano-"></div>
  <header>
    <Navbar />
  </header>
  <BackgroundText ></BackgroundText>
  <RouterView />
</template>

<style>
  #cristiano- {
    opacity: 0.66;
    position: absolute;
    width: 100%;
    height: 100%;
    background-image: url("@/assets/img/bg-img.png");
    background-repeat: no-repeat;
    background-attachment: scroll;
    z-index: 2;
  }
</style>
