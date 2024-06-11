<script setup lang="ts">

</script>

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
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  min-height: 100vh;
}
</style>
