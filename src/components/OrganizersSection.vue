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

    <div class="organizers mt-12">
      <a
        class="organizer"
        href="https://www.linkedin.com/in/anacarolinabarbosasilva/"
        target="_blank"
      >
        <img src="@/assets/organizers/Ana Silva.jpg" />
        <span class="name">Ana Silva</span>
        <span class="location">WTM SBC</span>
      </a>
      <a
        class="organizer"
        href="https://www.linkedin.com/in/aryelccapelo"
        target="_blank"
      >
        <img src="@/assets/organizers/Aryel Capelo.jpg" />
        <span class="name">Aryel Capelo</span>
        <span class="location">WTM & GDG SJC</span>
      </a>
      <a
        class="organizer"
        href="https://www.linkedin.com/in/fabicanedo/"
        target="_blank"
      >
        <img src="@/assets/organizers/Fabi Canedo Yugar.jpg" />
        <span class="name">Fabí Canedo</span>
        <span class="location">WTM SP</span>
      </a>
      <a
        class="organizer"
        href="https://www.linkedin.com/in/fehrezende/"
        target="_blank"
      >
        <img src="@/assets/organizers/Fernanda Rezende.jpg" />
        <span class="name">Fernanda Rezende</span>
        <span class="location">WTM & GDG BH</span>
      </a>
      <a
        class="organizer"
        href="https://www.linkedin.com/in/julianaconde/"
        target="_blank"
      >
        <img src="@/assets/organizers/Juliana Conde.jpg" />
        <span class="name">Juliana Conde</span>
        <span class="location">WTM Aparecida</span>
      </a>
      <a
        class="organizer"
        href="https://www.linkedin.com/in/leticialmoreira/"
        target="_blank"
      >
        <img src="@/assets/organizers/Leticia Moreira.jpg" />
        <span class="name">Letícia Moreira</span>
        <span class="location">WTM & GDG BH</span>
      </a>
      <a
        class="organizer"
        href="https://www.linkedin.com/in/tcrsilva/"
        target="_blank"
      >
        <img src="@/assets/organizers/Tais Silva.jpg" />
        <span class="name">Tais Silva</span>
        <span class="location">WTM Santos</span>
      </a>
    </div>

    <v-row style="width: 100vw" class="pa-12" justify="center">
      <v-col cols="12" lg="3" md="4" sm="6" xs="12">
        <v-card width="100%" class="px-5">
          <v-img :src="wtmLogo" class="align-end" height="200px"> </v-img>
        </v-card>
      </v-col>
      <v-col cols="12" lg="3" md="4" sm="6" xs="12">
        <v-card width="100%" class="px-5">
          <v-img :src="googleDevelopersLogo" class="align-end" height="200px">
          </v-img>
        </v-card>
      </v-col>
    </v-row>
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
  all: unset;
  display: flex;
  flex-direction: column;
  text-align: center;
  justify-content: center;
  align-items: center;
  gap: 0.5rem;
  margin: 0 auto;
  cursor: pointer;
}

.organizer img {
  width: 100%;
  border-radius: 100%;
}

.name {
  font-size: 0.875rem;
  color: var(--vt-c-blue);
  line-height: 18px;
  font-weight: 600;
}

.location {
  font-size: 0.7rem;
  line-height: 12px;
  color: var(--vt-c-black);
  font-weight: 600;
}

@media (min-width: 769px) {
  .organizer {
    width: 50%;
  }
}
</style>
