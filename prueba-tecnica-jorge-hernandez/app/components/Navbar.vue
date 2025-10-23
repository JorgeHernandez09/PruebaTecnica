<script setup>
import texts from "~/texts/text.json";
</script>

<template>
  <nav id="navbar" class="navbar">
    <div class="navbar__container">
      <a href="#" class="navbar__logo">{{ texts.navbar.logo }}</a>
      <div class="navbar__links">
        <a href="#hero" class="navbar__link">{{ texts.navbar.links.inicio }}</a>
        <a href="#about" class="navbar__link">{{
          texts.navbar.links.acercaDeMi
        }}</a>
        <a href="#technologies" class="navbar__link">{{
          texts.navbar.links.tecnologias
        }}</a>
        <a href="#experience" class="navbar__link">{{
          texts.navbar.links.experiencia
        }}</a>
        <a href="#projects" class="navbar__link">{{
          texts.navbar.links.proyectos
        }}</a>
        <a href="#contact" class="navbar__link">{{
          texts.navbar.links.contacto
        }}</a>
      </div>
      <a href="#">
        <img
          v-for="(image, index) in texts.navbar.icons"
          :key="index"
          :src="image"
          class="navbar__icons"
        />
      </a>
    </div>
  </nav>
</template>

<style scoped lang="scss">
@import "~/assets/styles/reset.scss";

.navbar {
  background-color: $background-dark;
  box-shadow: 0 0.125em 0.25em rgba(0, 0, 0, 0.2);
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  padding: 1em 2em;
  z-index: 1000;

  &__container {
    max-width: 95em;
    margin: 0 auto;
    display: grid;
    grid-template-columns: auto auto auto;
    align-items: center;
    position: relative;
  }

  &__logo {
    justify-self: center;
    font-size: 1.5em;
    font-weight: bold;
    color: $text-dark;
    text-decoration: none;
  }

  &__links {
    display: flex;
    gap: 2em;
    font-size: 1.15em;
    justify-self: center;

    @media (max-width: 48em) {
      position: absolute;
      top: 100%;
      left: 0;
      right: 0;
      background-color: $background-dark;
      flex-direction: column;
      align-items: center;
      display: none;
      padding: 1em 0;
    }
  }

  &__link {
    color: $text-dark;
    text-decoration: none;
    font-size: 0.8em;
    transition: color 0.3s ease;

    &:hover {
      color: $primary;
    }
  }

  &__icons {
    width: 2em;
    height: 2em;    
  }
}
</style>
