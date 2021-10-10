<template>
  <main class="bg-gray-100 p-6">
    <h1 class="text-4xl text-center">Vue Component</h1>

    <article class="space-y-4">

      <PropsComponent/>

      <PropsComponent :text="'Hey!'" />

      <EmitComponent @get-taco="getTaco"/>

      <SlotsComponent>
        <h3 class="text-xl font-bold">Hey</h3>
        <p>This is in a slot</p>
      </SlotsComponent>

      <SlotsComponent/>

    </article>
  </main>
</template>

<script>
  import PropsComponent from "./components/PropsComponent.vue";
  import EmitComponent from "./components/EmitComponent.vue";
  import SlotsComponent from "./components/SlotsComponent.vue";

  export default {
    components: {
      PropsComponent,
      EmitComponent,
      SlotsComponent
    },
    methods: {
      getTaco() {
        console.log("Taco");
      }
    }
  }
</script>