<template>
  <div class="mt-8 sm:mx-auto sm:w-full sm:max-w-md">
    <div class="bg-white py-8 px-4 shadow sm:rounded-lg sm:px-10">
      <p>{{ text }}</p>
    </div>
  </div>
</template>
<script>
export default {
  // props: ['text'], // This is simpler but the following is recommended
  props: {
    text: {
      type: String,
      default: 'Hello World'
    }
  },
}
</script>

