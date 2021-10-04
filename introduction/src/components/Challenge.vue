<template>
  <Card :title="'The Stupid Coach Challenge'">
    <!-- Todo: Recreate the Stupid Coach Challenge -->
    

    <input v-model="ask" id="name" name="name" type="text" autocomplete="off" required class="appearance-none block w-full px-3 py-2 border border-gray-300 rounded-md shadow-sm placeholder-gray-400 focus:outline-none focus:ring-indigo-500 focus:border-indigo-500 sm:text-sm" />
    <button @click="askStupidQuestion()" class="bg-blue-200 py-0.5 px-2 rounded-md">Ask!</button>
    <p class="text-gray-600 text-xs italic">{{ reply }}</p>

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
        ask: "What is the stupidest thing you've ever done?",
        reply: ""
      };
    },
    methods: {
      askStupidQuestion() {
        // Handle the stupid question 
        this.reply = "I don't care, get dressed and go to work!";
        if (this.ask.at(-1) === "?") this.reply = "Silly question, get dressed and go to work!";
      }
    }
  }
</script>