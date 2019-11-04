<template lang="html">

  <article class="openBook">
      <div class="content_book">
        <h1>{{title}}</h1>
        <small>7 Temas  |  Lectura 30 minutos </small><br>
        <small>By Rulótico González, Pedro carmona, Giglio pernima</small>
        <h2>1.Design and defining</h2>
        <p>Content</p>
      </div>
      <iframe width="100%" height="250px" src="https://www.youtube.com/embed/t1F_HhSAh_o" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
      <div class="content_book">

        <h2>1.Design and defining</h2>
        <p>Content</p>
        <h2>2.Design and defining</h2>
        <p>Content</p>
        <h2>3.Design and defining</h2>
        <p>Content</p>
      </div>
      <hr>
      <div class="content_book">
        <h2>4.Design and defining</h2>
        <p>Content</p>
        <h2>5.Design and defining</h2>
        <p>Content</p>
      </div>
  </article>

</template>

<script>
export default {
  props: {
    title: String,
  },
};
</script>

<style lang="css" scoped>
h1{
  font-size:2em;
}
small{
  color:var(--text);
}
.openBook .content_book{
  padding: var(--spacing);
}
.openBook{
  text-align:left;
  background-color: var(--white-color);
  box-shadow: var(--shadow);
  border-radius: 2px;
}
</style>
