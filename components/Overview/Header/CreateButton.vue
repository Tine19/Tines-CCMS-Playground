<template>
  <button @click="openDialog()">Create {{ getResourceName() }}</button>
  <!-- Create Dialog Includes -->
  <!-- Create Dialog Pages -->
</template>

<script lang="ts" setup>
import { defineProps } from 'vue';
const { resourceType } = defineProps<{
  resourceType?: string; // CCMSResourceType
}>();

function getResourceName() {
  // switch case to get translationkey or string for button name
  return resourceType || '';
}

function openDialog() {
  // switch case to open the correct create dialog
}
</script>
