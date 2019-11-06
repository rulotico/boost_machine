<template>
  <div class="home">
     <Title title="The knowledge you need for Software Development." />
     <router-link to="/design"><Book /></router-link>
     <router-link to="/design"><Book /></router-link>
     <router-link to="/design"><Book /></router-link>
     <router-link to="/design"><Book /></router-link>
     <router-link to="/design"><Book /></router-link>
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
