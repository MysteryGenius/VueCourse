<template>
  <Card :title="'Comment Component'">
    <!-- Todo: Use the v-for to display all the people in the people array -->
    <div>
      <ol>
        <li v-for="comment in comments" :key="comment.id" class="flex flex-col border-b">
          <span class="font-bold">{{ comment.name }}</span> 
          {{ comment.comment }}
        </li>
      </ol>
      <form class="flex mt-4 space-x-2" @submit.prevent="addComment">
        <input v-model.lazy="name" id="name" name="name" type="text" autocomplete="off" required class="appearance-none block w-full px-3 py-2 border border-gray-300 rounded-md shadow-sm placeholder-gray-400 focus:outline-none focus:ring-indigo-500 focus:border-indigo-500 sm:text-sm" placeholder="Name"/>
        <input v-model.lazy="comment" id="comment" name="comment" type="text" autocomplete="off" required class="appearance-none block w-full px-3 py-2 border border-gray-300 rounded-md shadow-sm placeholder-gray-400 focus:outline-none focus:ring-indigo-500 focus:border-indigo-500 sm:text-sm" placeholder="Comment"/>
        <button>Submit</button>
      </form>
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
        name: "",
        comment: "",
        comments: [
          {
            id: 1,
            name: "John Doe",
            comment: "This is a comment"
          },
          {
            id: 2,
            name: "Jane Doe",
            comment: "This is another comment"
          }
        ]
      }
    },
    methods: {
      addComment(){
        this.comments.push({
          id: this.comments.length + 1,
          name: this.name,
          comment: this.comment
        });
      }
    }
  }
</script>