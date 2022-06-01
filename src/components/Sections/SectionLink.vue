<template>
  <button @click="redirect" class="bg-mandy">
    {{ label }}
  </button>
</template>

<script>
export default {
  name: "SectionLink",
  props: {
    link: String,
    label: String,
  },
  methods: {
    redirect() {
      this.$emit("redirect", this.link);
    },
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/style.scss";

button {
  width: 100%;
  height: 150px;
  color: $white;
  border: 1px solid $mandy;
  text-transform: uppercase;
  font-size: 0.8rem;
  transition: 0.5s;

  &:hover {
    background: $white;
    color: $charade;
    border: 1px solid $white;
  }
}
</style>