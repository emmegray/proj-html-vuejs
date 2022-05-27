<template>
  <div class="main">

    <div class="jumbotron text-center">
      <h1 class="display-5 fw-bold">Untold Stories</h1>
      <div class="col-lg-6 mx-auto">
        <p class="lead mb-4 serif"><em>These is an untold story behind every favorite song.</em></p>
        <div class="d-grid gap-2 d-sm-flex justify-content-sm-center">
          <button type="button" class="btn-f btn-lg px-4 gap-3">Latest Album</button>
          <button type="button" class="btn-e btn-lg px-4">Live dates</button>
        </div>
      </div>
    </div>

    <section-container addClass="bg-ebony-clay">
      <section-header title="Music is Life"
        description="Lorem ipsum dolor sit amet consectetur, adipisicing elit. Laboriosam, beatae pariatur quod iste voluptatum provident? Possimus magnam nesciunt perspiciatis quisquam voluptatum fugiat, impedit magni. Dolores sequi accusantium quisquam quibusdam unde!" />
    </section-container>

    <section-container addClass="bg-charade">
      <section-header title="Latest Band News"
        description="Lorem ipsum dolor sit amet consectetur, adipisicing elit. Laboriosam, beatae pariatur quod iste voluptatum provident? Possimus magnam nesciunt perspiciatis quisquam voluptatum fugiat, impedit magni. Dolores sequi accusantium quisquam quibusdam unde!" />
    </section-container>

    <section-link link="#" label="View all latest news"></section-link>

  </div>
</template>

<script>
import SectionContainer from './Sections/SectionContainer.vue'
import SectionHeader from './Sections/SectionHeader.vue'
import SectionLink from './Sections/SectionLink.vue'

export default {
  components: { SectionContainer, SectionHeader, SectionLink },
  name: 'MainComp'
}
</script>

<style lang="scss" scoped>
@import "../assets/style.scss";

.jumbotron {
  background: url('../../public/img/home_slider.jpg') no-repeat center center;
  background-size: cover;
  height: 615px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
</style>