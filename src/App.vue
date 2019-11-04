<template>
  <div id="app">
    <NavBar />
    <Header />
    <div class="container">
      <OpenBook title="Design system"/>
      <router-view/>
    </div>
    <readBack />
    <Footer />
  </div>
</template>

<script>
// @ is an alias to /src
import NavBar from '@/components/NavBar.vue';
import Header from '@/components/Header.vue';
import readBack from '@/components/readBack.vue';
import Footer from '@/components/Footer.vue';

import OpenBook from '@/components/OpenBook.vue';

export default {
  name: 'home',
  components: {
    NavBar,
    Header,
    readBack,
    Footer,
    OpenBook,
  },
};
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
