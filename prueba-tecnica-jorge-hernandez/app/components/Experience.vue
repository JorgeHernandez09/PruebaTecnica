<script setup>
import texts from "~/texts/text.json";
</script>

<template>
  <section class="experience" id="experience">
    <div class="experience__container">
      <h2 class="experience__title">{{ texts.experience.title }}</h2>
      <div
        v-for="(job, index) in texts.experience.jobs"
        :key="index"
        class="experience__container--experiences"
      >
        <p class="experience__description--date">{{ job.date }}</p>
        <h3 class="experience__title--name">{{ job.position }}</h3>
        <p class="experience__subtitle">{{ job.company }}</p>
        <p class="experience__description">{{ job.description }}</p>
      </div>
    </div>
  </section>
</template>

<style scoped lang="scss">
@import "~/assets/styles/reset.scss";

.experience {
  min-height: 80dvh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  margin-bottom: 3em;
  padding: 2em 1em;

  &__container {
    display: flex;
    flex-direction: column;
    max-width: 40em;
    align-items: center;
    width: 100%;
    

    &--experiences {
      background-color: rgb(17 24 39);
      border-radius: 1em;
      width: 50em;
      max-width: 100%;
      height: 10em;
      max-height: 100%;
      padding: 2em;
      margin-bottom: 3em;
      text-align: left;
      box-shadow: 0 0.125em 0.25em rgba(0, 0, 0, 0.2);

      @media (max-width: 37.5em) {
        width: 100%;
        height: auto;
        padding: 1.5em;
      }
    }
  }

  &__title {
    font-size: 2em;
    margin-bottom: 1em;
    font-weight: bold;
    color: $text-dark;

    &--name {
      font-size: 1.25em;
      margin-bottom: 0em;
    }

    @media (max-width: 48em) {
      font-size: 1.5em;
    }
  }

  &__subtitle {
    font-size: 1em;
    font-weight: bold;
    color: $primary;
    margin-bottom: 1em;
  }

  &__description {
    font-size: 1em;
    max-width: 50em;
    color: #9ca3af;
    margin-bottom: 2em;

    &--date {
      font-size: 1em;
      color: #9ca3af;
      margin-bottom: 0;

      @media (max-width: 37.5em) {
        font-size: 1em;
      }
    }
  }
}
</style>
