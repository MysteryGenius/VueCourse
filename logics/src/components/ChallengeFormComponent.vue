<template>
  <Card :title="'Terrible Login Challenge Component'">
    <!-- Todo: Create a terrible login form -->
    <form class="flex mt-4 space-x-2">
      <input v-model.lazy="email" id="email" name="email" type="email" autocomplete="off" required class="appearance-none block w-full px-3 py-2 border border-gray-300 rounded-md shadow-sm placeholder-gray-400 focus:outline-none focus:ring-indigo-500 focus:border-indigo-500 sm:text-sm" placeholder="hello@example.com"/>
      <input v-model.lazy="password" id="password" name="password" type="password" autocomplete="off" required class="appearance-none block w-full px-3 py-2 border border-gray-300 rounded-md shadow-sm placeholder-gray-400 focus:outline-none focus:ring-indigo-500 focus:border-indigo-500 sm:text-sm" placeholder="Password"/>
      <button>Submit</button>
    </form>
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
        email: '',
        password: '',
        users: {
          dummy: {
            email: 'hello@vue.org',
            password: '123456'
          }
        }
      }
    },
    methods: {
      // Create a method for the form submit
    }
  }
</script>