<template>
  <div class="about">
    <CardInfo title="Who we are?" content="Example"/>
  </div>
</template>


<script>
// @ is an alias to /src
import CardInfo from '@/components/CardInfo.vue';

export default {
  name: 'home',
  components: {
    CardInfo,
  },
};
</script>
