<template>
  <main class="bg-gray-100 p-6">
    <h1 class="text-4xl text-center">Vue Directives</h1>

    <article class="space-y-4">
      <Dead/>

      <ModelComponent/>

      <IfElseComponent/>

      <Challenge/>
      
      <ForComponent/>

      <OnComponent/>
    </article>
  </main>
</template>

<script setup>
  import Dead from "./components/Dead.vue";
  import ModelComponent from "./components/ModelComponent.vue";
  import IfElseComponent from "./components/IfElseComponent.vue";
  import Challenge from "./components/Challenge.vue";
  import ForComponent from "./components/ForComponent.vue";
  import OnComponent from "./components/OnComponent.vue";
</script>