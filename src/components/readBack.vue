<template lang="html">
  <div class="readBack-container">
    <div class="readBack">
        You can try another book,
        <a href="#">
          <strong> Go Home</strong>
        </a>
    </div>
  </div>
</template>

<script>
export default {
  name:'readBack'
}
</script>

<style lang="css" scoped>
  .readBack-container{
    padding: 0 var(--spacing);
    height: 1em;
  }
  .readBack{
    background-color: var(--white-color);
    padding: 2em;
    box-shadow: var(--shadow);
    position: relative;
    border-radius: 2px;
  }
</style>
