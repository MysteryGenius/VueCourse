<template>
  <Card :title="'Computed Component'">
    <input v-model.lazy="name" id="email" name="email" type="email" autocomplete="off" required class="appearance-none block w-full px-3 py-2 border border-gray-300 rounded-md shadow-sm placeholder-gray-400 focus:outline-none focus:ring-indigo-500 focus:border-indigo-500 sm:text-sm" placeholder="What is your name?"/>
    <p>{{ greeting }}</p>
  </Card>
</template>

<script>
  import Card  from "./Card.vue";

  export default {
    components: {
      Card
    },
    computed: {
      greeting() {
        return `Hello! ${this.name}`;
      }
    },
    data() {
      return {
        name: ""
      }
    },
  }
</script>
