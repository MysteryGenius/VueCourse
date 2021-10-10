<template>
  <div class="mt-8 sm:mx-auto sm:w-full sm:max-w-md">
    <div class="bg-white py-8 px-4 shadow sm:rounded-lg sm:px-10">
      <h2 class="text-sm font-bold text-gray-600">
        Emit Component
      </h2>
      <div class="space-y-2 mt-4">
        <button @click="$emit('getTaco')" class="inline-flex items-center px-2.5 py-1.5 border border-transparent text-xs font-medium rounded shadow-sm text-white bg-indigo-600 hover:bg-indigo-700">
          Press for food
        </button>
      </div>
    </div>
  </div>
</template>
