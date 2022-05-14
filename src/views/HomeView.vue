<script setup lang="ts">
import TheWelcome from '@/components/TheWelcome.vue'
</script>

<template>
  <main>
    <TheWelcome />
  </main>
</template>

<style scoped lang="scss">
  main:after {
    content: "Yassdefzefzezfezfzefzefez";
    display: inline-block;
    width: 100%;
    z-index: 1;
  }
</style>