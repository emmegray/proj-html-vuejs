<template>
  <article>

    <div>
      <button @click="show" :class="{ open: showContent }">
        <font-awesome-icon v-if="showContent" icon="fa-solid fa-minus" size="m" />
        <font-awesome-icon v-else icon="fa-solid fa-plus" size="m" />
      </button>
      <h3>{{title}}</h3>
    </div>

    <div v-if="showContent">
      <slot></slot>
    </div>

  </article>
</template>

<script>
export default {
  name: "DateItem",
  props: {
    title: String,
  },
  data () {
    return {
      showContent: false
    }
  },
  methods: {
    show () {
      this.showContent = !this.showContent
    }
  }
};
</script>

<style lang="scss" scoped>
@import "../../assets/style.scss";

article {
  margin-bottom: 0.5rem;
  overflow: hidden;
}
div {
  text-align: left;
  background-color: $ebony-clay;
  padding: 10px;
}
div:first-child {
  display: flex;
  flex-direction: row;
  align-content: center;
  button {
    color: $white;
    border: 0;
    margin-right: 10px;
    background-color: transparent;
    &.open {
      background-color: $mandy;
    }
  }
  h3 {
    line-height: 1.5rem;
    margin: 0;
    text-transform: uppercase;
    color: $mandy;
    font-size: 1rem;
    font-weight: 300;
    letter-spacing: 1px;
  }
}
</style>