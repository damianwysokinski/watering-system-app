<template>
<!--  <app-sidebar />-->
<!--  <slot />-->

  <div class="antialiased">
    <!-- Sidebar -->
    <app-sidebar />

    <main class="p-4 ml-20 min-h-screen">
      <slot />
    </main>
  </div>
</template>

<script setup lang="ts">

</script>

<style scoped>

</style>