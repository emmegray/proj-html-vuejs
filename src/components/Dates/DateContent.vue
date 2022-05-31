<template>
  <div class="row">
    <div class="col-3">
      <img :src="`/img/${map}`" :alt="title" />
    </div>
    <article class="col-9 text">
      <section>
        <h4>{{ title }}</h4>
        <p>{{ description }}</p>
      </section>
      <section><button class="btn-f">book now</button></section>
    </article>
  </div>
</template>

<script>
export default {
  name: "DateContent",
  props: {
    title: String,
    description: String,
    map: String,
  },
};
</script>

<style scoped lang="scss">
@import "../../assets/style.scss";
.text {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  padding-left: 30px;
}
h4 {
  color: $white;
  font-size: 1rem;
  margin-bottom: 2rem;
  letter-spacing: 1px;
}
p {
  @extend .serif;
  color: $jumbo;
  line-height: 1.7rem;
}
.btn-f {
  padding: 5px 20px;
}
img {
  width: 100%;
}
</style>