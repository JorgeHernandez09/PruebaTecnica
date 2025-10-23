<script setup>
import texts from "~/texts/text.json";
</script>

<template>
  <section class="hero" id="hero">
    <div class="hero__container">
      <div class="photo__placeholder">
        <img class="hero__photo" :src="texts.hero.imageSrc "></img>
      </div>
      <div class="hero__container--text">
        <h1 class="hero__title">{{ texts.hero.title }}</h1>
        <p class="hero__subtitle">{{ texts.hero.subtitle }}</p>
        <p class="hero__description">{{ texts.hero.description }}</p>
        <a class="hero__button" href="#about">{{ texts.hero.button }}</a>
      </div>
    </div>
  </section>
</template>

<style scoped lang="scss">
@import "~/assets/styles/reset.scss";


.hero {
  min-height: 110dvh;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;

  &__container {
    max-width: 75em;
    display: flex;
    gap: 5em;
    align-items: center;
    flex-direction: row;
    text-align: left;
    
    &--text{
      max-width: 37em;
      display: flex;
      gap: 0em;
      align-items: left;
      flex-direction: column;
      text-align: left;
    }

    @media (max-width: 48em) {
      flex-direction: column;
      gap: 3em;
      text-align: center;
    }
  }

  &__title {
    font-size: 4.25em;
    font-weight: bold;
    margin-bottom: 0.1em;
    color: $text-dark;
    

    @media (max-width: 48em) {
      font-size: 3em;
    }
  }

  &__subtitle {
    font-size: 1.25em;
    margin-bottom: 1.5em;
    color: $text-dark;
    line-height: 1.25em;
  }

  &__description {
    font-size: 1em;
    color: #9ca3af;
    margin-bottom: 2em;
    line-height: 1.75em;
  }

    &__photo {
    background-color: $card-dark;
    border-radius: 50%;
    width: 18em;
    height: 18em;
    display: flex;
    align-items: center;
    justify-content: center;
    box-shadow: 0 0.625em 0.9375em rgba(0, 0, 0, 0.1);

    .photo-placeholder {
      color: #6b7280;
      font-size: 3em;
    }
  }

  &__button {
    background-color: $primary;
    color: #fff;
     max-width: 10em;
    font-weight: bold;
    padding: 0.75em 2em;
    border-radius: 0.5em;
    text-decoration: none;
    transition: background-color 0.3s ease;
    display: inline-block;
   

    &:hover {
      background-color: #0098d4dc;
    }
  }
}


</style>
