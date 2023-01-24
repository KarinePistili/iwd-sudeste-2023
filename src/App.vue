<script setup>
import { RouterView } from "vue-router";
</script>

<template>
  <header>
    <img class="logo" src="@/assets/web-banner.png" alt="Banner IWD 2023" />
    <h1 class="saveTheDateTitle">25 de março, 2023</h1>
    <h3 class="saveTheDateSubtitle">Presencial & Virtual</h3>
    <strong class="saveTheDatePlace">Google São Paulo | 13:00 - 18:00</strong>
  </header>

  <RouterView />

  <footer>
    <img class="img" src="@/assets/sticker-event.gif" alt="Social Gif IWD 2023" />
  </footer>
</template>

<style scoped>
@media (max-width: 1024px) {
  .saveTheDateTitle {
    visibility: hidden;
  }
  .saveTheDateSubtitle {
    visibility: hidden;
  }
  .saveTheDatePlace {
    visibility: hidden;
  }
}

@media (min-width: 1024px) {
  .img {
    width: 30%;
  }
}

.saveTheDateTitle {
  position: absolute;
  bottom: 150px;
  left: 40px;
  font-weight: 600;
}

.saveTheDateSubtitle {
  position: absolute;
  bottom: 110px;
  left: 40px;
  font-weight: 400;
}

.saveTheDatePlace {
  position: absolute;
  bottom: 70px;
  left: 40px;
  font-weight: 600;
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
