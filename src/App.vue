<script setup>
import { RouterView } from "vue-router";
</script>

<template>
  <header>
    <img class="logo" src="@/assets/web-banner.png" alt="Banner IWD 2023" />
  </header>

  <RouterView />

  <footer>
    <img src="@/assets/sticker-event.gif" alt="Social Gif IWD 2023" />
  </footer>
</template>

<style scoped>
header {
  width: 100%;
}

footer {
  margin: 40px 0;
  display: flex;
  justify-content: center;
}

footer img {
  width: 70%;
}

.logo {
  display: block;
  width: 100%;
}
</style>
