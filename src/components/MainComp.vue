<template>
  <div class="main">
    <jumbotron-container
      title="Untold Stories"
      description="These is an untold story behind every favorite song."
      addClass="bg-home-slider"
    >
      <button type="button" class="btn-f btn-lg px-4 gap-3">
        Latest Album
      </button>
      <button type="button" class="btn-e btn-lg px-4">Live dates</button>
    </jumbotron-container>

    <section-container addClass="bg-ebony-clay">
      <section-header
        title="Music is Life"
        description="Lorem ipsum dolor sit amet consectetur, adipisicing elit. Laboriosam, beatae pariatur quod iste voluptatum provident? Possimus magnam nesciunt perspiciatis quisquam voluptatum fugiat, impedit magni. Dolores sequi accusantium quisquam quibusdam unde!"
      />
    </section-container>

    <section-container addClass="bg-charade">
      <section-header
        title="Latest Band News"
        description="Lorem ipsum dolor sit amet consectetur, adipisicing elit. Laboriosam, beatae pariatur quod iste voluptatum provident? Possimus magnam nesciunt perspiciatis quisquam voluptatum fugiat, impedit magni. Dolores sequi accusantium quisquam quibusdam unde!"
      />
      <div class="row">
        <div class="col-8">
          <news-item
            size="small"
            image="blog_music_techo.jpg"
            text="Libero perspiciatis similique, minima nobis quis amet possimus ex aspernatur. Excepturi iusto suscipit veniam ex dolor minima eligendi assumenda magni voluptas odit."
            title="Technology and music"
          />
          <div class="row">
            <div class="col-6">
              <news-item
                size="big"
                image="blog-post3.jpg"
                text="Libero perspiciatis similique, minima nobis quis amet possimus ex aspernatur. Excepturi iusto suscipit veniam ex dolor minima eligendi assumenda magni voluptas odit."
                title="While my guitar gently weeps"
              />
            </div>
            <div class="col-6">
              <news-item
                size="big"
                image="blog-post4.jpg"
                text="Libero perspiciatis similique, minima nobis quis amet possimus ex aspernatur. Excepturi iusto suscipit veniam ex dolor minima eligendi assumenda magni voluptas odit."
                title="It just sounds better"
              />
            </div>
          </div>
          <news-item
            size="small"
            image="blog_flavor_rock.jpg"
            text="Libero perspiciatis similique, minima nobis quis amet possimus ex aspernatur. Excepturi iusto suscipit veniam ex dolor minima eligendi assumenda magni voluptas odit."
            title="The Flawor of rock"
          />
        </div>
        <div class="col-4">
          <news-item
            size="big"
            image="blog-post1.jpg"
            text="Libero perspiciatis similique, minima nobis quis amet possimus ex aspernatur. Excepturi iusto suscipit veniam ex dolor minima eligendi assumenda magni voluptas odit."
            title="Taking it back to the old school"
          />
          <news-item
            size="big"
            image="blog-post2.jpg"
            text="Libero perspiciatis similique, minima nobis quis amet possimus ex aspernatur. Excepturi iusto suscipit veniam ex dolor minima eligendi assumenda magni voluptas odit."
            title="Sharing the stage with a legend"
          />
        </div>
      </div>
    </section-container>

    <section-link link="#" label="View all latest news"></section-link>

    <jumbotron-container
      :description="`&quot; I just listened to it and said to myself, &quot;Man, I really love this
album.&quot; Still, today, it just sounds so fresh. It sounds full of ideas. These guys knew what they were doing. They're
      good. And they're inventive. I haven't heard anything this year that's as inventive. I don't really expect to.&quot;`"
      addClass="bg-home-testimonal"
    >
      <a href="#"
        ><img
          src="../../public/img/band_interview_play_icon.png"
          alt="play icon"
      /></a>
    </jumbotron-container>

    <section-container addClass="bg-charade">
      <section-header
        title="Live Dates"
        description="Lorem ipsum dolor sit amet consectetur, adipisicing elit. Laboriosam, beatae pariatur quod iste voluptatum provident? Possimus magnam nesciunt perspiciatis quisquam voluptatum fugiat, impedit magni. Dolores sequi accusantium quisquam quibusdam unde!"
      />
      <div class="py-5">
        <date-item title="17/08/2020 gem festival 2020 anakalia, georgia">
          <date-content
            description="Lorem ipsum dolor sit amet consectetur adipisicing elit. Eius molestias obcaecati neque quos, minus aliquam cum delectus consequuntur minima similique sint nulla quia rem totam at laborum enim natus fugit!"
            title="Untold Stories"
            map="fss-demo-main.jpg"
          />
        </date-item>
        <date-item title="24/9/2020 groovefest dominical republic">
          <date-content
            description="Lorem ipsum dolor sit amet consectetur adipisicing elit. Eius molestias obcaecati neque quos, minus aliquam cum delectus consequuntur minima similique sint nulla quia rem totam at laborum enim natus fugit!"
            title="Untold Stories"
            map="fss-demo-main.jpg"
          />
        </date-item>
        <date-item title="31/10/2020 oasis festival 2020 marrakech, morocco">
          <date-content
            description="Lorem ipsum dolor sit amet consectetur adipisicing elit. Eius molestias obcaecati neque quos, minus aliquam cum delectus consequuntur minima similique sint nulla quia rem totam at laborum enim natus fugit!"
            title="Untold Stories"
            map="fss-demo-main.jpg"
          />
        </date-item>
        <date-item title="07/11/2020 moga festival - essaouria, morocco">
          <date-content
            description="Lorem ipsum dolor sit amet consectetur adipisicing elit. Eius molestias obcaecati neque quos, minus aliquam cum delectus consequuntur minima similique sint nulla quia rem totam at laborum enim natus fugit!"
            title="Untold Stories"
            map="fss-demo-main.jpg"
          />
        </date-item>
        <date-item title="10/12/2020 envision festival - uvita, costa rica">
          <date-content
            description="Lorem ipsum dolor sit amet consectetur adipisicing elit. Eius molestias obcaecati neque quos, minus aliquam cum delectus consequuntur minima similique sint nulla quia rem totam at laborum enim natus fugit!"
            title="Untold Stories"
            map="fss-demo-main.jpg"
          />
        </date-item>
      </div>
    </section-container>

    <section-link link="#" label="View all live dates"></section-link>
  </div>
</template>

<script>
import DateItem from "./Dates/DateItem.vue";
import DateContent from "./Dates/DateContent.vue";
import JumbotronContainer from "./JumbotronContainer.vue";
import NewsItem from "./NewsItem.vue";
import SectionContainer from "./Sections/SectionContainer.vue";
import SectionHeader from "./Sections/SectionHeader.vue";
import SectionLink from "./Sections/SectionLink.vue";

export default {
  components: {
    SectionContainer,
    SectionHeader,
    SectionLink,
    JumbotronContainer,
    NewsItem,
    DateItem,
    DateContent,
  },
  name: "MainComp",
};
</script>

<style lang="scss" scoped>
@import "../assets/style.scss";

.bg-home-slider {
  background: url("../../public/img/home_slider.jpg") no-repeat center center;
}

.bg-home-testimonal {
  background: url("../../public/img/home-testimonial-parallax.jpg") no-repeat
    center center;
}
</style>