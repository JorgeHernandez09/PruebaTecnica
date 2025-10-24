<script setup>
import texts from "~/texts/text.json";
</script>

<template>
  <section class="projects" id="projects">
    <div class="projects__container">
      <h2 class="projects__title">{{ texts.projects.title }}</h2>
      <div class="projects__container--project">
        <div class="projects__container--project-primary" v-for="(project, index) in texts.projects.items" :key="index">
          <img :alt="project.imageAlt" class="projects__photo" :src="project.imageSrc || ''" />
          <h3 class="projects__subtitle">{{ project.title }}</h3>
          <p class="projects__description">{{ project.description }}</p>
          <a class="projects__button" href="#">{{ project.button }}</a>
        </div>
      </div>
    </div>
  </section>

</template>

<style scoped lang="scss">
@import "~/assets/styles/reset.scss";

.projects {
  min-height: 80dvh;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  background-color: rgb(17 24 39);

  &__container {
    display: flex;
    flex-direction: column;
    justify-content: center;
    margin-bottom: 3em;


    &--project {
      max-width: auto;
      margin: 1em;
      padding: 1em;
      display: flex;
      flex-direction: row;
      justify-content: center;
      gap: 8em;
      text-align: left;

      &-primary {
        padding: 1.5em;
        box-shadow: 0 0.125em 0.25em rgba(0, 0, 0, 0.6);
        border-radius: 2em;

      &:hover{
        box-shadow: 0 0.125em 0.25em rgba(1, 225, 255, 0.6);
      }
      }
    }

  }

  &__title {
    font-size: 2.5em;
    font-weight: bold;
    margin-bottom: 2em;
    color: $text-dark;
  }

  &__subtitle {
    font-size: 1.5em;
    font-weight: bold;
    color: $text-dark;
  }

  &__description {
    font-size: 1em;
    color: #9ca3af;
    margin-bottom: 2em;
  }

  &__button {
    color: #0098d4dc;
    font-size: 1em;
    text-decoration: none;
    align-items: end;

    &:hover {
      text-decoration: underline;
    }
  }

  &__photo {
    background-color: $card-dark;
    border-radius: 2em;
    width: 25em;
    height: 20em;
    display: flex;
    align-items: center;
    justify-content: center;
    box-shadow: 0 0.625em 0.9375em rgba(0, 0, 0, 0.1);

    .photo-placeholder {
      color: #6b7280;
    }
  }
}
</style>