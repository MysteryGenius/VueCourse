<template>
  <Card :title="'The v-model directive'">
    <!-- Todo: Use the v-model to bind the input to a data variable -->

    <label for="name" class="block text-sm font-medium text-gray-700">Name</label>
    <input v-model="name" id="name" name="name" type="text" autocomplete="off" required class="appearance-none block w-full px-3 py-2 border border-gray-300 rounded-md shadow-sm placeholder-gray-400 focus:outline-none focus:ring-indigo-500 focus:border-indigo-500 sm:text-sm" />

    <p>Hey my name is {{ name }}!</p>
  </Card>
</template>

<script>
  import Card  from "./Card.vue";

  export default {
    components: {
      Card
    },
    data() {
      return {
        name: 'Jian Zhen'
      }
    }
  }
</script>