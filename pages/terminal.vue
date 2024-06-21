<template>
  <app-breadcrumb :links="links" />
</template>

<script setup lang="ts">
const links = [
  {
    label: 'Terminal',
    to: '/terminal'
  }
];
</script>

<style scoped>

</style>