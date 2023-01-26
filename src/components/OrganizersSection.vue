<script setup>
import Title from "./SectionTitle.vue";
import wtmLogo from "../assets/wtm-logo.png";
import googleDevelopersLogo from "../assets/google-developers-group.png";
</script>

<script>
export default {
  data: () => ({
    wtmLogo,
    googleDevelopersLogo,
  }),
};
</script>

<template>
  <section>
    <Title text="Organização" />
    <v-row style="width: 100vw" class="pa-12" justify="center">
      <v-col cols="12" lg="3" md="4" sm="6" xs="12">
        <v-card width="100%" class="px-5">
          <v-img :src="wtmLogo" class="align-end" height="200px"> </v-img>
        </v-card>
      </v-col>
      <v-col cols="12" lg="3" md="4" sm="6" xs="12">
        <v-card width="100%" class="px-5">
          <v-img :src="googleDevelopersLogo" class="align-end" height="200px"> </v-img>
        </v-card>
      </v-col>
    </v-row>
    <div class="organizers mt-12">
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
