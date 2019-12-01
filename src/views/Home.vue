<template>
  <div class="home">
     <Title title="The knowledge you need for Software Development" />
     <router-link to="/design">

       <Book
        title="Design system collaboration workflow"
        description="Process, stylish and control frames"
        img="book.png"
        v-bind:themes="[
        'Design and defining',
        'Construct the system',
        'Appeal the perfect',
        'Procedural definition',
        'Know How',
        'Simple as that'
        ]"
        />


     </router-link>

  </div>
</template>

<script>
// @ is an alias to /src
import Book from '@/components/Book.vue';
import Title from '@/components/Title.vue';

export default {
  name: 'home',
  components: {
    Book,
    Title,
  },
};
</script>
