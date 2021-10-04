<template>
  <Card :title="'The v-if directive'">
    <!-- Todo: Use the v-model to bind the input to a data variable -->
    <div class="relative flex items-start">
      <div class="flex items-center h-5">
        <input @click="checked = !checked" id="offers" aria-describedby="offers-description" name="offers" type="checkbox" class="focus:ring-indigo-500 h-4 w-4 text-indigo-600 border-gray-300 rounded" />
      </div>
      <div class="ml-3 text-sm">
        <label class="font-bold text-green-700" v-if="checked">Checked</label>
        <label class="font-bold text-red-700" v-else>Unchecked</label>
      </div>
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
        checked: true
      }
    }
  }
</script>