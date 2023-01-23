<script setup>
import Title from "./SectionTitle.vue";
</script>

<template>
  <section>
    <Title text="Data e Local" />
    <span class="date"><strong>25 de Março</strong></span>
    <span class="location">
      <strong>Google SP | 13:00 - 18:00</strong>
    </span>
  </section>
</template>

<style scoped>
.date {
  font-size: 1rem;
}

.location {
  font-size: 0.875rem;
  color: var(--vt-c-blue);
}
</style>
