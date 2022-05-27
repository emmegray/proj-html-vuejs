<template>
  <div class="header container-fluid">
    <img class="logo" src="../assets/img/avada-music-logo.png" alt="logo">
    <font-awesome-icon icon="fa-solid fa-bars" />
  </div>
</template>

<script>
export default {
  name:'HeaderComp'
}
</script>

<style lang="scss" scoped>
.header {
  box-sizing: content-box;
  height: 115px;
  overflow: visible;
  width: 100%;
  justify-content: space-around;
  padding: 20px 20px;
}


</style>