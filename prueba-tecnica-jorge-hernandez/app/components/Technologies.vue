<script setup>
import texts from "~/texts/text.json";
</script>

<template>
  <section class="technologies" id="technologies">
    <div class="technologies__container">
      <h2 class="technologies__title">{{ texts.technologies.title }}</h2>
      <div class="technologies__container--languages">
        <p
          v-for="(language, index) in texts.technologies.languages"
          :key="index"
          class="technologies__subtitle"
        >
          {{ language }}
          <img
            :src="texts.technologies.imageSrc[index]"
            class="technologies__photo"
          />
        </p>
      </div>
    </div>
  </section>
</template>

<style scoped lang="scss">
@import "~/assets/styles/reset.scss";

.technologies {
  min-height: 30em;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
  background-color: rgb(17 24 39);
  margin-bottom: 1em;

  &__container {
    margin-top: 0;
    margin-bottom: 2em;
    width: 100%;
    max-width: 75em;
    display: flex;
    flex-direction: column;
    align-items: center;

    &--languages {
      display: grid;
      grid-template-columns: auto auto auto auto;
      gap: 10em;
      column-gap: 20em;
      justify-content: center;

      @media (max-width: 48em) {
        grid-template-columns: auto auto;
        gap: 4em;
      }

      @media (max-width: 30em) {
        grid-template-columns: 1fr;
        gap: 2em;
      }
    }
  }

  &__title {
    font-size: 2.5em;
    font-weight: bold;
    color: $text-dark;
    line-height: 1.75em;
    margin-bottom: 1.5em;
  }

  &__subtitle {
    font-size: 1.25em;
    font-weight: bold;
    color: $text-dark;
    line-height: 1.75em;
    margin-bottom: 1.5em;
  }

  &__photo {
    background-color: $card-dark;
    width: 4em;
    height: 4em;
    display: flex;
    align-items: center;
    justify-content: center;
  }
}
</style>
