<script setup>
import Title from "./SectionTitle.vue";
</script>

<template>
  <section>
    <Title text="Data e Local" />
    <span class="date"><strong>25 de Março | 13:00 - 18:00</strong></span>
    <span class="location">
      <strong>Escritório Google São Paulo</strong>

      <p style="font-size:1.2rem">Av. Brg. Faria Lima, 3477 - Itaim Bibi, São Paulo - SP, 04538-133;</p>
    </span>
  </section>
</template>

<style scoped>
.date {
  font-size: 1.2rem;
}

.location {
  font-size: 1.3rem;
  color: var(--vt-c-blue);
  text-align: center;
}

section {
  margin-top: 60px;
}
</style>
