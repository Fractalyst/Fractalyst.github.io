<script setup lang="ts">
import AutoScrollingText from '@/components/AutoScrollingText.vue';
import LanguageBlock from '@/components/LanguageBlock.vue';


</script>

<template>
  <div class="home-view">
    <div class="scrolling-container">
      <AutoScrollingText />
    </div>
    <LanguageBlock class="objective-container">
      <main>
        <h1 style="margin-left: 5px;">Objectives</h1>
        <ul>
          <li>Continuously adapt to ensure project requirements are completely fulfilled.</li>
          <li>Collaborate and engage with team members to share knowledge.</li>
          <li>To work with people by learning their specific needs to make a plan tailored for their use.</li>
          <li>Apply this understanding and transform it into diverse solutions both practical and technical.</li>
        </ul>
      </main>
    </LanguageBlock>
  </div>
</template>

<style scoped>
.home-view {
  justify-content: right;
  display: flex;
  height: 500px;
  place-content: center;
  align-items: center;
}

.scrolling-container {
  width: 600px;
  height: 500px;
  z-index: 99;
}

.objective-container {
  background-color: var(--vt-c-white-soft);
  width: 500px;
  height: 300px;
  margin-left: -10%;
  z-index: 100;
}

@media (prefers-color-scheme: dark) {
  .objective-container {
    background-color: var(--vt-c-black-soft);
  }
}
</style>
