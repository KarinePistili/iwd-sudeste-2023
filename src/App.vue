<script setup>
import { RouterView } from "vue-router";
import Footer from "./components/Footer.vue";
</script>

<template>
  <v-app>
    <header>
      <img class="logo" src="@/assets/web-banner.svg" alt="Banner IWD 2023" />
    </header>

    <RouterView />

    <Footer />
  </v-app>
</template>

<style scoped>
@media (min-width: 1024px) {
  .img {
    width: 30%;
  }
}

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
