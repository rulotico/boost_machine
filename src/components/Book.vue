<template lang="html">
  <article class="book">
    <div class="feature">
      <div class="text-feature">
        System testing configuration
      </div>

    </div>
    <div class="shadow">

    </div>

    <div class="info">
      <h3>A nice approach to design systems and how to build it and defining</h3>
      <ul>
        <li>Design and defining</li>
        <li>Construct the system</li>
        <li>Appeal the perfect</li>
        <li>Procedural definition</li>
        <li>Know How</li>
        <li>Simple as that</li>
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
  li{
    list-style-type: circle;
    list-style-position: inside;
    padding: 2px 0;
  }
  h3{
    margin-top: 0;
    font-size: 17px;
    font-weight: 400;
    color:var(--text);
  }
  .book{
    background-color: var(--white-color);
    margin-top: var(--spacing);
    box-shadow: var(--shadow);
    display: flex;
    border-radius: var(--radius);
  }
  .feature{
    /* background-color: salmon; */
    background: url(~@/assets/book.png) center center;
    background-size: cover;
    border-radius:var(--radius) 0 0 var(--radius);
    font-weight: bold;
    text-align: left;
    color: var(--white-color);
    display: inherit;
  }
  .shadow{
    background-color: black;
    height: 100px;
    width: calc(50% - var(--spacing));
    position: absolute;
    bottom: calc(0px + var(--spacing));
    opacity: 0.4;
    background: linear-gradient(transparent, black);
  }
  .text-feature{
    margin-top: auto;
    position: relative;
    z-index: 2;
    text-shadow: 1px 1px black;
  }
  .info{
    text-align: left;
  }

  .feature, .info{
    width: calc(50% - var(--spacing) - var(--spacing));
    padding: var(--spacing)
  }

</style>
