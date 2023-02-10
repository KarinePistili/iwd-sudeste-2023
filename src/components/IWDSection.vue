<script setup>
import Title from "./SectionTitle.vue";
import instagramIcon from "../assets/instagram.png";
import linkedinIcon from "../assets/linkedin.png";
</script>

<script>
export default {
  data: () => ({
    instagramIcon,
    linkedinIcon,
  }),
  methods: {
    goTo(url) {
      window.open(url);
    },
  },
};
</script>

<template>
  <section>
    <Title text="O que é IWD?" />
    <p class="content">
      O Dia Internacional da Mulher (IWD) é a maior campanha anual de eventos da
      Women Techmakers, onde as Embaixadoras realizam eventos em todo o mundo
      durante os meses de março e abril em comemoração a este momento.
    </p>
    <p class="content">
      De grandes cúpulas a reuniões menores e íntimas, o IWD é um momento para
      criarmos conexões, compartilhar conhecimento e inspirar nós mulheres e
      comunidades de tecnologia. É também uma forma de apoiarmos nossa missão de
      construir um mundo onde todas as mulheres prosperem juntas.
    </p>

    <p class="content">
      Em 2022, nossa campanha <strong>#ProgressNotPerfection</strong> IWD alcançou mais de 132
      mil participantes em todo o mundo. Em 2023, nosso objetivo é superar este
      número!
    </p>
    <p class="content">
      Siga nossas redes sociais para informações dos eventos que virão!
    </p>

    <v-row>
      <v-col>
        <div
          class="socialContainer"
          @click="goTo('https://www.instagram.com/iwdsudeste/')"
        >
          <img height="50" :src="instagramIcon" />
          <h4 class="url">@iwdsudeste</h4>
        </div>
      </v-col>
      <v-col>
        <div
          class="socialContainer"
          @click="
            goTo('https://www.linkedin.com/company/women-techmakers-sudeste/')
          "
        >
          <img height="50" :src="linkedinIcon" />
          <h4 class="url">Women Techmakers Sudeste</h4>
        </div>
      </v-col>
    </v-row>
  </section>
</template>

<style scoped>
.content {
  font-size: 1.1rem;
}
.socialContainer {
  text-align: center;
  cursor: pointer;
}

.url {
  margin-top: 10px;
  color: var(--vt-c-blue);
}
</style>
