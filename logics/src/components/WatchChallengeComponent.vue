<template>
  <Card :title="'Watch Challenge Component'">
    <!-- Todo: Use watch on counter to console log the old value and the new value -->
    <div>
      <input v-model="counter" id="counter" name="counter" type="number" autocomplete="off" required class="appearance-none block w-full px-3 py-2 border border-gray-300 rounded-md shadow-sm placeholder-gray-400 focus:outline-none focus:ring-indigo-500 focus:border-indigo-500 sm:text-sm" placeholder="Comment"/>
      <p class="text-center">{{ counter }}</p>
    </div>
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
        counter: 0

      }
    },
    watch: {
    }
  }
</script>
