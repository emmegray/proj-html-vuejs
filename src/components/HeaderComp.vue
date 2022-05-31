<template>
  <nav class="header">
    <img class="logo" src="/img/avada-music-logo.png" alt="logo" />
    <button @click="show">
      <font-awesome-icon v-if="showMenu" icon="fa-solid fa-xmark" size="xl" />
      <font-awesome-icon v-else icon="fa-solid fa-bars" size="xl" />
    </button>

    <div class="menu" :class="{ show: showMenu }">
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">Mee The Band</a></li>
        <li><a href="#">Live Dates</a></li>
        <li><a href="#">Latest News</a></li>
        <li><a href="#">Albums</a></li>
        <li><a href="#">Fans</a></li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {
  name: "HeaderComp",
  data: function () {
    return {
      showMenu: false,
    };
  },
  methods: {
    show() {
      this.showMenu = !this.showMenu;
      document.body.style.overflow = this.showMenu ? "hidden" : "visible";
    },
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/style.scss";

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
  z-index: 5;
  overflow: visible;
}
.logo,
button {
  z-index: 7;
}
button {
  background: transparent;
  border: 0;
  color: $white;
}
.menu {
  top: 0;
  left: 0;
  z-index: 6;
  height: 100vh;
  width: 100vw;
  position: fixed;
  background-color: $mandy;
  align-items: center;
  justify-content: center;
  text-align: center;
  display: flex;
  opacity: 0;
  transition: opacity ease-in 0.5s;
  pointer-events: none;
  &.show {
    opacity: 1;
    pointer-events: all;
  }
}
ul li {
  margin-bottom: 3rem;
}

ul li a {
  font-size: 2rem;
  color: white;
  opacity: 0.5;
  &:hover {
    opacity: 1;
  }
}

.fa-xmark {
  padding-right: 17px;
}
</style>