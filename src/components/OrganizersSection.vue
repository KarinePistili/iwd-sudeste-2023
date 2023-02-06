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
        href="https://www.linkedin.com/in/alice-ribeiro-280812182/"
        target="_blank"
      >
        <img src="@/assets/organizers/AliceRibeiro.jpg" />
        <span class="name">Alice Ribeiro</span>
        <span class="location">WTM & GDG Lavras</span>
      </a>
      <a
        class="organizer"
        href="https://www.linkedin.com/in/anacarolinabarbosasilva/"
        target="_blank"
      >
        <img src="@/assets/organizers/AnaSilva.jpg" />
        <span class="name">Ana Silva</span>
        <span class="location">WTM SBC</span>
      </a>
      <a
        class="organizer"
        href="https://www.linkedin.com/in/aryelccapelo"
        target="_blank"
      >
        <img src="@/assets/organizers/AryelCapelo.jpg" />
        <span class="name">Aryel Capelo</span>
        <span class="location">WTM & GDG SJC</span>
      </a>
      <a
        class="organizer"
        href="https://www.linkedin.com/in/fabicanedo/"
        target="_blank"
      >
        <img src="@/assets/organizers/FabiCanedoYugar.jpg" />
        <span class="name">Fabí Canedo</span>
        <span class="location">WTM SP</span>
      </a>
      <a
        class="organizer"
        href="https://www.linkedin.com/in/fernandacosta-tech"
        target="_blank"
      >
        <img src="@/assets/organizers/FernandaCosta.jpg" />
        <span class="name">Fernanda Costa</span>
        <span class="location">WTM SP</span>
      </a>
      <a
        class="organizer"
        href="https://www.linkedin.com/in/fehrezende/"
        target="_blank"
      >
        <img src="@/assets/organizers/FernandaRezende.jpg" />
        <span class="name">Fernanda Rezende</span>
        <span class="location">WTM & GDG BH</span>
      </a>
      <a
        class="organizer"
        href="https://www.linkedin.com/in/gabuldev/"
        target="_blank"
      >
        <img src="@/assets/organizers/GabrielSavio.png" />
        <span class="name">Gabriel Sávio</span>
        <span class="location">GDG BH</span>
      </a>
      <a
        class="organizer"
        href="https://www.linkedin.com/in/isabella-soares-lima/"
        target="_blank"
      >
        <img src="@/assets/organizers/IsabellaLima.jpg" />
        <span class="name">Isabella Lima</span>
        <span class="location">WTM Sorocaba</span>
      </a>
      <a
        class="organizer"
        href="https://www.linkedin.com/in/julianaconde/"
        target="_blank"
      >
        <img src="@/assets/organizers/JulianaConde.jpg" />
        <span class="name">Juliana Conde</span>
        <span class="location">WTM Aparecida</span>
      </a>
      <a
        class="organizer"
        href="https://www.linkedin.com/in/karine-pistili/"
        target="_blank"
      >
        <img src="@/assets/organizers/KarinePistili.png" />
        <span class="name">Karine Pistili</span>
        <span class="location">WTM & GDG Sorocaba</span>
      </a>
      <a
        class="organizer"
        href="https://www.linkedin.com/in/leticialmoreira/"
        target="_blank"
      >
        <img src="@/assets/organizers/LeticiaMoreira.jpg" />
        <span class="name">Letícia Moreira</span>
        <span class="location">WTM & GDG BH</span>
      </a>
      <a
        class="organizer"
        href="https://www.linkedin.com/in/maisa-ceruti"
        target="_blank"
      >
        <img src="@/assets/organizers/MaisaCeruti.png" />
        <span class="name">Maísa Ceruti</span>
        <span class="location">WTM & GDG SJC</span>
      </a>
      <a
        class="organizer"
        href="https://www.linkedin.com/in/maizalouise/"
        target="_blank"
      >
        <img src="@/assets/organizers/MaizaLouise.jpg" />
        <span class="name">Maiza Louise</span>
        <span class="location">GDG Bauru</span>
      </a>
      <a
        class="organizer"
        href="https://www.linkedin.com/in/nicolerachid/"
        target="_blank"
      >
        <img src="@/assets/organizers/NicoleRachid.png" />
        <span class="name">Nicole Rachid</span>
        <span class="location">WTM SP</span>
      </a>
      <a
        class="organizer"
        href="https://www.linkedin.com/in/tcrsilva/"
        target="_blank"
      >
        <img src="@/assets/organizers/TaisSilva.jpg" />
        <span class="name">Tais Silva</span>
        <span class="location">GDG & WTM Santos</span>
      </a>
      <a
        class="organizer"
        href="https://www.linkedin.com/in/victor-pugliese-1bb568168"
        target="_blank"
      >
        <img src="@/assets/organizers/VictorPugliese.png" />
        <span class="name">Victor Pugliese</span>
        <span class="location">GDG Caraguatatuba</span>
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

span {
  all: unset;
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
  justify-content: flex-start;
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
