<template>
  <app-breadcrumb :links="links" />

  <div v-if="error" class="flex items-center p-4 mb-4 text-sm text-red-800 border border-red-300 rounded-lg bg-red-50" role="alert">
    <svg class="flex-shrink-0 inline w-4 h-4 me-3" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="currentColor" viewBox="0 0 20 20">
      <path d="M10 .5a9.5 9.5 0 1 0 9.5 9.5A9.51 9.51 0 0 0 10 .5ZM9.5 4a1.5 1.5 0 1 1 0 3 1.5 1.5 0 0 1 0-3ZM12 15H8a1 1 0 0 1 0-2h1v-3H8a1 1 0 0 1 0-2h2a1 1 0 0 1 1 1v4h1a1 1 0 0 1 0 2Z"/>
    </svg>
    <span class="sr-only">Info</span>
    <div>
      <span class="font-medium">Device doesn't work!</span> Calibrate water tank volume.
    </div>
  </div>

  <div class="grid grid-cols-4 gap-4 mb-4">
    <div
        class="p-2 bg-white border rounded-md border-gray-200 text-center"
    >
      <div class="text-base">
        Total Days
      </div>
      <div class="font-bold text-2xl">
        76
      </div>
    </div>
    <div
        class="p-2 bg-white border rounded-md border-gray-200 text-center"
    >
      <div class="text-base">
        Temperature
      </div>
      <div class="font-bold text-2xl my-auto">
        26°C
      </div>
    </div>
    <div
        class="p-2 bg-white border rounded-md border-gray-200 text-center"
    >
      <div class="text-base">
        Air Humidity
      </div>
      <div class="font-bold text-2xl">
        56%
      </div>
    </div>
    <div
        class="p-2 bg-white border rounded-md border-gray-200 text-center"
    >
      <div class="text-base">
        Soil Humidity
      </div>
      <div class="font-bold text-2xl">
        20%
      </div>
    </div>
  </div>

  <div class="grid grid-cols-4 gap-4 mb-4 bg-white border rounded-md border-gray-200 ">
    <div
        class="p-2 text-center border-r border-gray-200"
    >
      <div>
        <div>Temperature</div>
        <div>MAX: 26°C</div>
        <div>MIN: 26°C</div>
        <div>AVG: 26°C</div>
      </div>
    </div>

    <div class="p-2 col-span-3">

    </div>
  </div>

  <div class="grid grid-cols-4 gap-4 bg-white border rounded-md border-gray-200">
    <div
        class="p-2 text-center border-r border-gray-200"
    >
      <div>
        <div>Air Humidity</div>
        <div>MAX: 76%</div>
        <div>MIN: 76%</div>
        <div>AVG: 76%</div>
      </div>
    </div>

    <div class="p-2 col-span-3">

    </div>
  </div>
</template>

<script setup lang="ts">
const links = [
  {
    label: 'Home',
    to: '/'
  }
];

const error = ref(false);
</script>

<style scoped>

</style>