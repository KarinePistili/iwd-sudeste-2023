<script setup>
import Title from "./SectionTitle.vue";
</script>

<template>
  <section>
    <Title text="Organização" />
    <div class="organizers">
      <div class="organizer">
        <img src="@/assets/organizer-profile.png" />
        <span>Ambassador name</span>
      </div>
      <div class="organizer">
        <img src="@/assets/organizer-profile.png" />
        <span>Ambassador name</span>
      </div>
      <div class="organizer">
        <img src="@/assets/organizer-profile.png" />
        <span>Ambassador name</span>
      </div>
      <div class="organizer">
        <img src="@/assets/organizer-profile.png" />
        <span>Ambassador name</span>
      </div>
      <div class="organizer">
        <img src="@/assets/organizer-profile.png" />
        <span>Ambassador name</span>
      </div>
      <div class="organizer">
        <img src="@/assets/organizer-profile.png" />
        <span>Ambassador name</span>
      </div>
    </div>
  </section>
</template>

<style scoped>
section {
  margin-top: 40px;
}

.organizers {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-gap: 24px;
}

.organizer {
  display: flex;
  flex-direction: column;
  text-align: center;
  justify-content: center;
  align-items: center;
  font-size: 0.875rem;
  color: var(--vt-c-blue);
}
</style>
