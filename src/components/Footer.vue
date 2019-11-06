<template lang="html">
  <footer>
    <p>You can meet us in
      <a href="https://hnmexico.herokuapp.com/" target="_blank">
        <strong>Hacker News México</strong>
        <span class="slack-img">
          <img :src="img" alt="">
        </span>
      </a>

    </p>
    <a href="#" class="legals">Privacy</a>
    <a href="#" class="legals">Terms of service</a>
  </footer>
</template>

<script>
import foot1 from '../assets/slack.svg';

export default {
  name: 'Footer',
  data() {
    return {
      img: foot1,
    };
  },
};
</script>

<style lang="css" scoped>
  footer{
    background: url(~@/assets/foot.svg) top center;
    background-size: 101%;
    padding: 4em var(--spacing) var(--spacing) var(--spacing);
    text-align: left;
  }
  footer p{
    color:var(--white-color);
  }
  footer a{
    padding-right: 1em;
    color:var(--white-color);
  }
  .slack-img{
    position: relative;
    top: 1.5px;
    left: 5px;
  }
  .legals{
    font-size: 10px;
  }
</style>
