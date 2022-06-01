<template>
  <section class="py-5">
    <h2 class="fw-bold">{{ title }}</h2>
    <div class="separator"></div>
    <p class="serif">
      {{ description }}
    </p>
  </section>
</template>

<script>
export default {
  name: "SectionHeader",
  props: {
    title: String,
    description: String,
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/style.scss";

h2 {
  font-size: 3rem;
}

h2,
p {
  margin: 0;
  padding: 0;
}

p {
  color: $tapa;
}

.separator {
  margin-top: 1.5rem;
  margin-bottom: 1.5rem;
  display: inline-block;
  width: 240px;
  border-bottom: 1px solid $tapa;
}
</style>