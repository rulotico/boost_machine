<template lang="html">
    <div class="">
      <h1>{{ title }}</h1>
      <div class="icon animated fadeIn" v-if="[':name'].includes($route.name)">
        <img :src="icon" alt="" >
      </div>
    </div>
</template>

<script>
import icon from '../assets/big_icon.svg';

export default {
  name: 'Title',
  data() {
    return {
      icon,
    };
  },
  props: {
    title: String,
  },
};
</script>

<style lang="css" scoped>
  h1{
    color:var(--white-color);
    text-shadow: 1px 1px 4px #626263;
    margin-bottom: 0px;
  }
  .icon{
    padding: var(--spacing)
  }
</style>
