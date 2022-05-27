<template>
  <nav class="header">
    <img class="logo" src="/img/avada-music-logo.png" alt="logo">
    <font-awesome-icon icon="fa-solid fa-bars" size="xl" />
  </nav>
</template>

<script>
export default {
  name: 'HeaderComp'
}
</script>

<style lang="scss" scoped>
.header {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 90px;
  padding: 0px 20px 0px;
  text-align: start;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;
  z-index: 1000;
}
</style>