<template>
  <div id="app">
    <NavBar />
    <Header />
    <div class="container">
      <Title />
      <CardInfo />
      <Book />
    </div>
    <readBack />
    <Footer />

  </div> <!-- **/app -->
</template>

<script>
  import NavBar from './components/NavBar.vue'
  import Header from './components/Header.vue'
  import Title from './components/Title.vue'
  import CardInfo from './components/CardInfo.vue'
  import Book from './components/Book.vue'
  import readBack from './components/readBack.vue'
  import Footer from './components/Footer.vue'

  export default {
    name: 'app',
    components: {
      NavBar,
      Header,
      Title,
      CardInfo,
      Book,
      readBack,
      Footer
    },
    data(){
      return{
        leng:true
      }
    }
  }
</script>

<style>
  :root {
    --primary-color: #F3F90D;
    --white-color: white;
    --text:#626977;
    --black-color:#272323;
    --shadow:0 0 7px 0px #00000030;
    --spacing:1.5em;
    --radius:2px;
  }

  body{
    background-color: var(--primary-color);
    margin:0px;
  }
  h1{
    text-align: left;
    margin-top: 0px;
    color: var(--black-color);
  }
  p{
    text-align: justify;
    color: var(--text)
  }
  ul{
    color: var(--text);
  }
  a{
    text-decoration: none;
  }
  p a,div a,footer a{
    color: var(--black-color);

  }
  nav a, footer a{
    text-decoration: none;
  }
  ul{
    margin:0px;
  }
  /* HELPERS */
  .container{
    padding: var(--spacing);
    position: relative;
    padding-top: 3em;
  }
  #app {
    font-family: 'Noto Sans JP', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
  }
</style>
