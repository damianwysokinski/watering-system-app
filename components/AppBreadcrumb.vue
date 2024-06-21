<template>
  <nav class="flex mb-4" aria-label="Breadcrumb">
    <ol class="inline-flex items-center space-x-1 md:space-x-2 rtl:space-x-reverse">
      <li v-for="({ label, to }, index) in links" :key="index" class="inline-flex items-center">
        <NuxtLink :to="to" class="inline-flex items-center text-sm font-medium text-gray-400">
          {{ label }} /
        </NuxtLink>
      </li>
    </ol>
  </nav>
</template>

<script setup lang="ts">
defineProps({
  links: Array,
});
</script>

<style scoped>

</style>