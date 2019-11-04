<template>
  <div class="leng-btn" @click="changeLeng" >
    <div class="tracker-l">
      <div class="tracker-l-btn">

      </div>
    </div>
    <div class="switcher-flags">
      <div class="usa">🇺🇸</div>
      <div class="mexico">🇲🇽</div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'LenguageSwitcher',
  methods: {
    changeLeng() {
      if (this.active) {
        this.$emit('false');
      } else {
        this.$emit('true');
      }
    },
  },
};
</script>

<style>

.leng-btn{
  cursor: pointer;
}

.switcher-flags{
  width: 60px;
  height: 30px;
  font-size: 11px;
  box-shadow: 0 0 6px 0px rgba(64, 62, 62, 0.23137254901960);

  align-items: center;
  display: flex;
  justify-content: space-around;
  background-color: #B4B4B4;
  border-radius: 2px;
}
.usa,.mexico{
  position: relative;
  z-index: 2;
}
.tracker-l{
  height: 0px;
  z-index: 2;
  position: relative;
  transition: 1s ease all;
}
.leng-btn.active .tracker-l{
  margin-left: 30px;
}

.tracker-l-btn{
  background-color: white;
  height: 30px;
  width: 30px;
  border-radius: 2px;
  box-shadow: 0 0 6px 0px rgba(64, 62, 62, 0.23137254901960);
}

</style>
