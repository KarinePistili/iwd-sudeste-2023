<script setup>
import Title from "./SectionTitle.vue";
import LectureComponent from "./LectureComponent.vue";
</script>

<template>
  <section>
    <Title text="Agenda" />

    <!-- <LectureComponent
      time="12:00 - 14:00"
      description="Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
            eiusmod tempor incididunt ut labore et dolore magna aliqua."
      speaker="Speaker"
    />

    <LectureComponent
      time="14:00 - 16:00"
      description="Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
            eiusmod tempor incididunt ut labore et dolore magna aliqua."
      speaker="Speaker"
    /> -->
    <span>Em breve!</span>
  </section>
</template>

<style scoped>
.lecture {
  display: flex;
  gap: 44px;
  font-size: 0.875rem;
}

.time {
  text-align: center;
}

.description p {
  text-align: left;
}

.description span {
  font-size: 0.75rem;
}

.time,
.description span {
  color: var(--vt-c-blue);
  font-weight: 500;
}

img {
  height: 4px;
  width: 100%;
}

span {
  font-size: 1.2rem;
  font-weight: 500;
}

section {
  margin-top: 60px;
}
</style>
