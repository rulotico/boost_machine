<template>
  <div class="about">
    <Title title=""/>
    <OpenBook title="Design system"/>
  </div>
</template>


<script>
// @ is an alias to /src
import OpenBook from '@/components/OpenBook.vue';
import Title from '@/components/Title.vue';


export default {
  name: 'home',
  components: {
    OpenBook,
    Title,
  },
};
</script>
