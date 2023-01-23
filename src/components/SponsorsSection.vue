<script setup>
import Title from "./SectionTitle.vue";
</script>

<template>
  <section>
    <Title text="Patrocinadores" />
    <div class="sponsors">
      <img src="@/assets/sponsors.png" />
      <img src="@/assets/sponsors.png" />
      <img src="@/assets/sponsors.png" />
      <img src="@/assets/sponsors.png" />
      <img src="@/assets/sponsors.png" />
      <img src="@/assets/sponsors.png" />
    </div>
  </section>
</template>

<style scoped>
section {
  margin-top: 0;
}
.sponsors {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-gap: 24px;
}
</style>
