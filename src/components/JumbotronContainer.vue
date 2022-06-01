<template>
  <div :class="`jumbotron text-center ${addClass}`">
    <h1 class="display-5 fw-bold">{{ title }}</h1>
    <div class="col-lg-6 mx-auto">
      <p class="lead mb-4 serif">
        <em>{{ description }}</em>
      </p>
      <div class="d-grid gap-2 d-sm-flex justify-content-sm-center">
        <slot></slot>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "JumbotronContainer",
  props: {
    title: String,
    description: String,
    addClass: String,
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/style.scss";

.jumbotron {
  background-color: $charade;
  background-size: cover;
  height: 615px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
</style>