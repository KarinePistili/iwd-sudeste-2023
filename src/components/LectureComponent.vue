<script setup>
defineProps({
  description: {
    type: String,
    required: true,
  },
  speaker: {
    type: String,
    required: true,
  },
  time: {
    type: String,
    required: true,
  },
});
</script>

<template>
  <div>
    <div class="lecture">
      <div class="time">{{ time }}</div>
      <div class="description">
        <p>
          {{ description }}
        </p>
        <span>{{ speaker }}</span>
      </div>
    </div>

    <img src="@/assets/line.jpg" />
  </div>
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
</style>
