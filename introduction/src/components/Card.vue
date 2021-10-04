<template>
  <div class="mt-8 sm:mx-auto sm:w-full sm:max-w-md">
    <div class="bg-white py-8 px-4 shadow sm:rounded-lg sm:px-10">
      <h2 class="text-sm font-bold text-gray-600">
        {{ title }}
      </h2>
      <div class="space-y-2 mt-4">
        <slot></slot>
      </div>
    </div>
  </div>
</template>

<script setup>
  defineProps({
    title: String
  });
</script>