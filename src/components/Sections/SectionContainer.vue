<template>
  <div :class="`section-container text-center ${addClass}`">
    <div class="container">
      <slot></slot>
    </div>
  </div>
</template>

<script>
export default {
  name: "SectionContainer",
  props: {
    addClass: String,
  },
};
</script>

<style>
</style>