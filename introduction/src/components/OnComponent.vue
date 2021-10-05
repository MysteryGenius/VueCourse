<template>
  <Card :title="'The v-on directive'">
    <!-- Todo: Use the v-on to create a toggle -->
    <p @click="checked = !checked">{{ checked }}</p>
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
        checked: false,
      };
    },
  };
</script>

<style>
</style>