<template lang="html">
  <article class="book">
    <div class="feature">
      feature
    </div>
    <div class="info">
      <h3>A nice approach to design systems and how to build it and defining</h3>
      <ul>
        <li>Design and defining</li>
        <li>Design and defining</li>
        <li>Design and defining</li>
        <li>Design and defining</li>
        <li>Design and defining</li>
        <li>Design and defining</li>
        <li>Design and defining</li>
      </ul>
    </div>
  </article>
</template>

<script>
export default {
  name:'Book'
}
</script>

<style lang="css" scoped>
  ul{
    padding-left: 0;
    font-size: 10px;
  }
  .book{
    background-color: var(--white-color);
    margin-top: var(--spacing);
    box-shadow: var(--shadow);
    display: flex;
    border-radius: var(--radius);
  }
  .feature{
    background-color: salmon;
    border-radius:var(--radius) 0 0 var(--radius);
  }
  .info{
    text-align: left;
  }

  .feature, .info{
    width: calc(50% - var(--spacing) - var(--spacing));
    padding: var(--spacing)
  }
</style>
