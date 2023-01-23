<script setup>
defineProps({
  text: {
    type: String,
    required: true,
  },
});
</script>

<template>
  <div class="section-title">
    <h2>{{ text }}</h2>
    <img src="@/assets/line.jpg" />
  </div>
</template>

<style scoped>
.section-title {
  width: fit-content;
}

h2 {
  font-weight: 600;
  font-size: 1rem;
  text-align: center;
  margin-bottom: -12px;
}

.section-title img {
  height: 4px;
  width: 100%;
}
</style>
