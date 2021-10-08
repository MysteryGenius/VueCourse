<template>
  <Card :title="'Watched Component'">
    <div>

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
      counter() {
        console.log("counter changed");
      }
    }
  }
</script>
