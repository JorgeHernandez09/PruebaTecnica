<script setup>
import texts from "~/texts/text.json";
</script>

<template>
    <section class="about" id="about">
        <div class="about__container">
            <h2 class="about__title">{{ texts.about.title }}</h2>
            <h3 class="about__subtitle--name">{{ texts.about.name }}</h3>
            <p class="about__description">{{ texts.about.description1 }}</p>
            <h4 class="about__subtitle">{{ texts.about.interestsTitle }}</h4>
            <p class="about__description">{{ texts.about.description2 }}</p>
            <a class="about__button" href="#projects">{{ texts.about.button }}</a>
        </div>
    </section>
</template>

<style scoped lang="scss">
@import "~/assets/styles/reset.scss";


.about {
    min-height: 75dvh;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    text-align: center;
    margin-bottom: 2.5em;

    &__container {
        display: flex;
        flex-direction: column;
        max-width: 75em;
        align-items: center;
        text-align: center;
    }

    &__title {
        font-size: 2em;
        font-weight: bold;
        margin-bottom: 1em;
        color: $text-dark;
    }

    &__subtitle {
        font-size: 1.25em;
        margin-bottom: 0em;
        color: $text-dark;

        &--name {
            font-size: 1.25em;
            color: $primary;
            margin-bottom: 0em;
        }
    }

    &__description {
        font-size: 1em;
        tab-size: 60;
        max-width: 50em;
        color: #9ca3af;
        margin-bottom: 2em;
        line-height: 1.75em;
        tab-size: 4;
    }

    &__button {
        background-color: $primary;
        color: white;
        font-weight: bold;
        padding: 0.75em 2em;
        border-radius: 0.5em;
        text-decoration: none;
        transition: background-color 0.3s ease;

        &:hover {
            background-color: #0098d4dc;
        }
    }
}
</style>