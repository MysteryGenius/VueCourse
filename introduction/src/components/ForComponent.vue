<template>
  <Card :title="'The v-for directive'">
    <!-- Todo: Use the v-for to display all the people in the people array -->
    <ul>
      <li v-for="person in people" :key="person.text">{{ person.text }}</li>
    </ul>
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
        people: [
          {
            text: "Sam"
          },
          {
            text: "Josh"
          },
          {
            text: "Nadia"
          }
        ]
      };
    },
  };
</script>