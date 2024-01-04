<template>
  <AppNavbar />
  <!-- hero section -->
  <section class="atevadd-hero">
    <div class="atevadd-hero__container">
      <div class="atevadd-hero__text">
        <h2>Hi, I'm Tofunmi</h2>
        <h1>Frontend Developer</h1>
        <p>
          I build pixel perferct, responsive, user-friendly, high-performance
          website that is accessible to all, helping individuals and businesses
          achieve their goals.
        </p>
      </div>
      <div class="atevadd-hero__img">
        <img src="@/assets/images/portrait.jpg" alt="" />
      </div>
    </div>
  </section>

  <!-- value section -->
  <section class="atevadd-value">
    <div class="atevadd-value__container">
      <div class="value" v-for="value in content.values">
        <h3>{{ value.heading }}</h3>
        <p>{{ value.body }}</p>
      </div>
    </div>
  </section>

  <!-- About section -->
  <section class="atevadd-about">
    <div class="atevadd-about__title">
      <h2>
        About <br />
        me
      </h2>
    </div>
    <div class="atevadd-about__content">
      <p>
        I started my coding journey some years back, and ever since then it has
        been an amazing experience. Over the years, I have worked on different
        types of website ranging from ecommerce websites, to landing pages to
        corporate website. While on this projects I have worked with UI designer
        and backend developers to bring some of these projects to life.
      </p>
      <div class="ruler"></div>
      <p>
        When I am not coding I enjoy reading, teaching and taking long walks
        becoming aware of my environment. I'm constantly finding ways of
        improving myself, by reading that tech blog post, watching that youtube
        video and shorts, and going through that instagram carousel.
      </p>
      <div class="ruler"></div>

      <p>I currently work at Voyatekgroup</p>
    </div>
  </section>
</template>

<script setup>
import AppNavbar from "../components/AppNavbar.vue";
import * as content from "../content.json";
</script>

<style lang="scss" scoped></style>
