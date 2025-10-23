<script setup>
import texts from "~/texts/text.json";
</script>

<template>

      <section class="contact" id="contact">
      <div class="contact__container">
        <h2 class="contact__title">{{ texts.contact.title }}</h2>
        <p class="contact__description">{{ texts.contact.description }}</p>
        <form action="#" method="post" class="contact__container--form">
          <label class="contact__subtitle" for="name">
            {{ texts.contact.form.labels.name }}
          </label>
          <input
            class="contact__form"
            id="name"
            name="name"
            :placeholder="texts.contact.form.placeholders.name"
            type="text"
            required
          />

          <label class="contact__subtitle" for="email">
            {{ texts.contact.form.labels.email }}
          </label>
          <input
            class="contact__form"
            id="email"
            name="email"
            :placeholder="texts.contact.form.placeholders.email"
            type="email"
            required
          />

          <label class="contact__subtitle" for="message">
            {{ texts.contact.form.labels.message }}
          </label>
          <textarea
            class="contact__form"
            id="message"
            name="message"
            :placeholder="texts.contact.form.placeholders.message"
            rows="4"
            required
          ></textarea>

          <button class="contact__button" type="submit">
            {{ texts.contact.form.button }}
          </button>
        </form>
      </div>
    </section>

</template>



<style scoped lang="scss">
@import "~/assets/styles/reset.scss";


.contact {
  min-height: 60dvh;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  margin: 2em 0;

  &__container {
    display: flex;
    width: 38em;
    flex-direction: column;
    justify-content: center;
    margin-bottom: 3em;

    &--form {
      display: flex;
      flex-direction: column;
      justify-content: center;
      margin-bottom: 3em;
    }
  }

  &__title {
    font-size: 2.5em;
    font-weight: bold;
    color: $text-dark;
  }

  &__subtitle {
    text-align: left;
    font-size: 1em;
    color: #9ca3af;
    margin-top: 1.5em;
  }

  &__description {
    font-size: 1.25em;
    color: #9ca3af;
  }

  &__form {
    color:white;
    border: 0.0625em solid #4b5563;
    background-color: #1f2937;
    border-radius: 0.5em;
    height: 3em;
    margin-top: 0.25em;
    padding-left: 1em;
    font-size: 1em;

    &:hover {
      border-color: #0098d4dc;
    }
  }

  &__button {
    background-color: $primary;
    color: white;
    font-weight: 600;
    width: 15em;
    height: 4em;
    border: none;
    padding: 0.75em 2em;
    align-self: center;
    border-radius: 0.5em;
    text-decoration: none;
    transition: background-color 0.3s ease;
    margin-top: 3em;

    &:hover {
      background-color: #0098d4dc;
    }
  }
}



</style>