<script setup lang="ts">
import { RouterView } from 'vue-router'
import PageHeader from './components/PageHeader.vue';
</script>

<template>
  <header>
    <PageHeader />
  </header>
  <div class="view">
    <RouterView />
  </div>
</template>

<style scoped>
header {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
}

@media (min-width: 768px) {
  .view {
    display: grid;
    grid-template-columns: 1fr 1fr;
    padding: 64px 2rem 0;
  }
}
</style>
