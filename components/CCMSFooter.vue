<script setup lang="ts">
// TODO add logic for footer context info (sorting, etc) depending on route and state --> composable
</script>

<template>
  <footer class="tchibo-footer">
    <span>Some infos about sorting stuff</span>
    <span>copyright &copy;</span>
  </footer>
</template>

<style scoped>
.tchibo-footer {
  width: 100%;
  background-color: gold;
  padding: 1em;
  display: flex;

  span {
    margin: 0 1em;
  }
}
</style>
