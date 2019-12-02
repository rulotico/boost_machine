<template lang="html">
  <article class="book animated fadeIn">
    <div class="feature"
      :style="{'background-image': 'url(' + require('../assets/covers/'+ imagebook +'') + ')'}" >
      <div class="text-feature">
        {{title}}
      </div>

    </div>
    <div class="shadow">

    </div>

    <div class="info">
      <h3>{{description}}</h3>
      <ul id="example-1">
        <ul v-for="item in themes" :key="item">
          <li>{{ item }}</li>
        </ul>
      </ul>
    </div>
  </article>
</template>

<script>

export default {


  name: 'Book',
  props: {
    title: String,
    description: String,
    imagebook: String,
    themes: Array,
  },
};
</script>

<style lang="css" scoped>
  ul{
    padding-left: 0;
    font-size: 11px;
  }
  li{
    list-style-type: circle;
    list-style-position: inside;
    padding: 2px 0;
  }
  h3{
    margin-top: 0;
    font-size: 14px;
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
    background-color: var(--black-color) !important;
    /* background-image: url('~@/assets/book.png'); */
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
    font-size: 17px;
    text-shadow: 0 0 6px black;
  }
  .info{
    text-align: left;
  }

  .feature, .info{
    width: calc(50% - var(--spacing) - var(--spacing));
    padding: var(--spacing)
  }

</style>
