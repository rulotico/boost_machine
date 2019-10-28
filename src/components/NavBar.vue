<template>
  <nav>
    <div class="logo">
      <img :src="img" alt="">
    </div>
    <ul class="options">
      <li>
        <a href="#">
        Us
        </a>
      </li>
      <li>
        <LenguageSwitcher />
      </li>
    </ul>
  </nav>
</template>

<script>
import LenguageSwitcher from './LenguageSwitcher.vue'
export default {
  name: 'NavBar',
  components:{
    LenguageSwitcher
  },
  data(){
    return{
      img:"logo.png"
    }
  }
}
</script>

<style>

nav{
  display: flex;
  justify-content: space-between;
  padding: var(--spacing);
  align-items: center;
  position: relative;
  z-index: 2;
}

nav .logo img{
  height: 2em;
  max-height: 70px;
}

.options{
  display: flex;
}

li{
  padding: 0 5px;
  list-style: none;
}

li a{
      font-size: 12px;
      text-decoration: none;
      color: black;
}

</style>
