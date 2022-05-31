<template>
  <article :class="size">
    <img :src="`/img/${image}`" :alt="title" />
    <div class="overlay">
      <span>{{ title }}</span>
    </div>
    <div class="text">
      <h3>{{ title }}</h3>
      <p>{{ text }}</p>
    </div>
  </article>
</template>

<script>
export default {
  name: "NewsItem",
  props: {
    image: String,
    title: String,
    text: String,
    size: String,
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/style.scss";

article {
  position: relative;
  overflow: hidden;
  flex-direction: column;
  text-align: left;
  align-items: center;
  margin-bottom: 27px;

  &.small {
    height: 325px;
    img {
      width: 100%;
    }
  }
  &.big {
    height: 680px;
    img {
      height: 100%;
    }
  }
}
.text {
  position: absolute;
  bottom: 0;
  width: 100%;
  padding: 1.2rem;
  background-color: $ebony-clay;
  z-index: 2;
  transition: transform ease-in 0.5s ;
}
.overlay {
  position: absolute;
  height: 100%;
  width: 100%;
  top: 0;
  left: 0;
  z-index: 2;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  display: flex;
  opacity: 0;
  transition: opacity ease-in 0.5s ;
  &:hover {
    opacity: 0.8;
    background: $mandy;
  }
  &:hover+.text {
    transform: translateY(100%);
  }
  span {
    letter-spacing: 2px;
    font-size: 1.2rem;
  }
}

h3 {
  color: $mandy;
  font-size: 1.5rem;
}
p {
  color: $mid-gray;
  margin: 0;
  padding: 0;
  @extend .serif;
}
</style>