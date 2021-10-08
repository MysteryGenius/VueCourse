<template>
  <main class="bg-gray-100 p-6">
    <h1 class="text-4xl text-center">Vue Logics</h1>

    <article class="space-y-4">

      <ColourComponent/>
      
      <CommentComponent/>

      <ChallengeFormComponent/>

      <ComputedComponent/>

    </article>
  </main>
</template>

<script setup>
  import ColourComponent from "./components/ColourComponent.vue";
  import CommentComponent from "./components/CommentComponent.vue";
  import ChallengeFormComponent from "./components/ChallengeFormComponent.vue";
  import ComputedComponent from "./components/ComputedComponent.vue";
</script>