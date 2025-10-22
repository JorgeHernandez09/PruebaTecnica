<script lang="ts" setup>
import texts from "~/texts/text.json";
</script>

<template>
<footer class="footer">
    <div class="footer__container">
      <p>{{ texts.footer.copyright }}</p>
      <div class="footer__social">
        <a class="footer__link" :href="texts.footer.socialLinks.github">
        </a>
        <a class="footer__link" :href="texts.footer.socialLinks.linkedin">
        </a>
      </div>
    </div>
  </footer>
</template>



<style scoped lang="scss">
@import "~/assets/styles/reset.scss";



.footer {
    background-color: $background-dark;
    padding: 1.5rem 1rem;
    border-top: 1px solid #374151; 

    &__container {
        max-width: 1280px;
        margin: 0 auto;
        text-align: center;
        color: #9ca3af;
    }

    &__social {
        display: flex;
        justify-content: center;
        gap: 1rem;
        margin-top: 1rem;
    }

    &__link {
        color: inherit;
        transition: color 0.3s ease;

        &:hover {
            color: $primary;
        }
    }
}


</style>