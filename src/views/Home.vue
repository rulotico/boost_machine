<template>
  <div class="home">
    <Title title="The knowledge you need for Software Development." />
     <Book />
     <Book />
     <Book />
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
