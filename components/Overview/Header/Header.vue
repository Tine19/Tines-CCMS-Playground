<template>
  <div class="header">
    <div v-if="false">Topic wrapper to implement</div>
    <div>Tabs to implement</div>
    <OverviewHeaderSearch />
    <OverviewHeaderSorting />
    <OverviewHeaderCreateButton :resourceType="selectedResource" />
  </div>
</template>

<script lang="ts" setup>
const selectedResource = computed(
  () => 'Page' /* calculate from route param */
);
</script>

<style>
.header {
  background: orange;
  padding: 1rem 0;
  display: flex;
  justify-content: space-between;
}
</style>
