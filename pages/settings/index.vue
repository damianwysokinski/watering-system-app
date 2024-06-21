<template>
  <div>
    <app-breadcrumb :links="links" />
<!--    <div>-->
<!--      <div class="uppercase font-medium">Grow Time</div>-->
<!--      <div>Total Days: 13</div>-->
<!--      <div>Flowering: not started</div>-->
<!--      <NuxtLink-->
<!--          to="/settings/grow-time"-->
<!--          class="inline-block text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:ring-blue-300 font-medium rounded-md text-sm px-5 py-2.5 mt-2 focus:outline-none"-->
<!--      >-->
<!--        Edit-->
<!--      </NuxtLink>-->
<!--    </div>-->
  </div>
</template>

<script setup lang="ts">
const links = [
  {
    label: 'Settings',
    to: '/settings'
  }
];
</script>

<style scoped>

</style>