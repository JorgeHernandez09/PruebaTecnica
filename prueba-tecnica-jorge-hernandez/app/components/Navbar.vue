<script setup>
import texts from "~/texts/text.json";
</script>

<template>
  <nav id="navbar" class="navbar">
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
      <a href="#"  class="navbar__icons">
        <img
          v-for="(image, index) in texts.navbar.icons"
          :key="index"
          :src="image"
        />
      </a>
  </nav>
</template>

<style scoped lang="scss">
@import "~/assets/styles/reset.scss";

.navbar {
  background-color: $background-dark;
  box-shadow: 0 0.125em 0.25em rgba(0, 0, 0, 0.175);
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  padding: 0.75em 2em;
  z-index: 1000;

  max-width: 100%;
    display: grid;
    grid-template-columns: repeat(3, auto);
    align-items: center;



  &__logo {
    justify-self: left;
    padding: 0 2.5em;
    font-size: 1.5em;
    font-weight: bold;
    color: $text-dark;
    text-decoration: none;
  }

  &__links {
    display: flex;
    gap: 1.25em;
    font-size: 1.15em;
    justify-self: left;
    padding: 0 3em;
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
    display: flex;
    flex-direction: row;
    justify-self: center;
    padding: 0 2em 0 0;
    gap: 0.5em;
  }
}
</style>
