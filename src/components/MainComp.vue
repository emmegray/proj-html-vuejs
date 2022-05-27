<template>
  <div class="main">

    <jumbotron-container title="Untold Stories" description="These is an untold story behind every favorite song."
      addClass="bg-home-slider">
      <button type="button" class="btn-f btn-lg px-4 gap-3">Latest Album</button>
      <button type="button" class="btn-e btn-lg px-4">Live dates</button>
    </jumbotron-container>

    <section-container addClass="bg-ebony-clay">
      <section-header title="Music is Life"
        description="Lorem ipsum dolor sit amet consectetur, adipisicing elit. Laboriosam, beatae pariatur quod iste voluptatum provident? Possimus magnam nesciunt perspiciatis quisquam voluptatum fugiat, impedit magni. Dolores sequi accusantium quisquam quibusdam unde!" />
    </section-container>

    <section-container addClass="bg-charade">
      <section-header title="Latest Band News"
        description="Lorem ipsum dolor sit amet consectetur, adipisicing elit. Laboriosam, beatae pariatur quod iste voluptatum provident? Possimus magnam nesciunt perspiciatis quisquam voluptatum fugiat, impedit magni. Dolores sequi accusantium quisquam quibusdam unde!" />
    </section-container>

    <section-link link="#" label="View all latest news"></section-link>

    <jumbotron-container
      :description="`&quot; I just listened to it and said to myself, &quot;Man, I really love this
album.&quot; Still, today, it just sounds so fresh. It sounds full of ideas. These guys knew what they were doing. They're
      good. And they're inventive. I haven't heard anything this year that's as inventive. I don't really expect to.&quot;`"
      addClass="bg-home-testimonal">
      <a href="#"><img src="../../public/img/band_interview_play_icon.png" alt="play icon"></a>
    </jumbotron-container>
  </div>
</template>

<script>
import JumbotronContainer from './JumbotronContainer.vue'
import SectionContainer from './Sections/SectionContainer.vue'
import SectionHeader from './Sections/SectionHeader.vue'
import SectionLink from './Sections/SectionLink.vue'

export default {
  components: { SectionContainer, SectionHeader, SectionLink, JumbotronContainer },
  name: 'MainComp'
}
</script>

<style lang="scss" scoped>
@import "../assets/style.scss";

.bg-home-slider {
  background: url('../../public/img/home_slider.jpg') no-repeat center center;
}

.bg-home-testimonal {
  background: url('../../public/img/home-testimonial-parallax.jpg') no-repeat center center;
}
</style>