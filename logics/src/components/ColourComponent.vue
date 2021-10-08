<template>
  <Card :title="'Pastel Colour Component'">
    <!-- Todo: Use the v-for to display all the people in the people array -->
    <div @mousemove="xCoordinate" :style="{ backgroundColor: `hsl(${x}, 70%, 80%)` }" class="h-72 w-80 mx-auto rounded-xl shadow-xl border-8"></div>
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
        x: 0
      }
    },
    methods: {
      xCoordinate(event) {
        this.x = event.clientX + event.clientY;
      }
    }
  }
</script>