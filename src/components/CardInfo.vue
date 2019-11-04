<template lang="html">
    <article class="cardInfo">
      <h1 class="title">
        {{ title }}
      </h1>
      <p>{{content}}</p>

    </article>
</template>

<script>
export default {
  name: 'CardInfo',
  props: {
    title: String,
    content: String,
  },
};
</script>

<style lang="css" scoped>
.cardInfo{
  padding: var(--spacing);
  background-color: var(--white-color);
  box-shadow: var(--shadow);
  border-radius: 2px;
}
</style>
