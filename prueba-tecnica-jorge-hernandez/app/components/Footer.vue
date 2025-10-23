<script lang="ts" setup>
import texts from "~/texts/text.json";
</script>

<template>
<footer class="footer">
    <div class="footer__container">
      <p>{{ texts.footer.copyright }}</p>
      <div class="footer__social">
        <a href="#">
        <img
          v-for="(image, index) in texts.footer.icons"
          :key="index"
          :src="image"
          class="footer__icons"
        />
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
  &__icons {
    width: 2em;
    height: 2em;    
  }
}


</style>