<script setup>
import IWDSection from "../components/IWDSection.vue";
import DareToBeSection from "../components/DareToBeSection.vue";
import SubscriptionButton from "../components/SubscriptionButton.vue";
import SpeakersSection from "../components/SpeakersSection.vue";
import AgendaSection from "../components/AgendaSection.vue";
import LocationSection from "../components/LocationSection.vue";
import SponsorsSection from "../components/SponsorsSection.vue";
import OrganizersSection from "../components/OrganizersSection.vue";
</script>

<template>
  <main>
    <v-container>
      <IWDSection />
      <!-- <img class="line" src="@/assets/line.jpg" /> -->
      <DareToBeSection />
      <!-- <SubscriptionButton /> -->
      <SpeakersSection />
      <AgendaSection />
      <LocationSection />
      <!-- <SubscriptionButton /> -->
      <SponsorsSection class="mt-12" />
      <OrganizersSection />
    </v-container>
  </main>
</template>

<style scoped>
main {
  padding: 0 16px;

  display: flex;
  flex-direction: column;
  align-items: center;
}

.line {
  height: 4px;
  width: 100%;
  margin-top: 50px;
}
</style>
