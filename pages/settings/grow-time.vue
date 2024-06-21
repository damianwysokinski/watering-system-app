<template>
  <div>
    <app-breadcrumb :links="links" />
  </div>
</template>

<script setup lang="ts">
const links = [
  {
    label: 'Settings',
    to: '/settings'
  },
  {
    label: 'Grow Time',
    to: '/settings/grow-time'
  }
];
</script>

<style scoped>

</style>