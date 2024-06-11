<script setup lang="ts"></script>

<template>
  <div class="root-container">
    <div class="main" role="main">
      <slot />
    </div>
    <CCMSFooter />
  </div>
</template>

<style scoped>
.root-container {
  display: grid;
  grid-template:
    'content' 97%
    'footer';
  min-height: 100vh;
}

.main {
  padding: 1%;
  background: lightblue;
}
</style>
