<template lang="html">
    <div class="">
      <h1>{{ title }}</h1>
      <div class="icon">
        <!-- <img :src="icon" alt=""> -->
      </div>
    </div>
</template>

<script>
import icon from '../assets/big_icon.png';
export default {
  name:'Title',
  data(){
    return{
      title:"The knowledge you need for Software development",
      icon:icon
    }
  }
}
</script>

<style lang="css" scoped>
  h1{
    color:var(--white-color);
    text-shadow: 1px 1px 4px #626263;
    margin-bottom: 0px;
  }
  .icon{
    padding: var(--spacing)
  }
</style>
