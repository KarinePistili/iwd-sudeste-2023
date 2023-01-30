<script setup>
import Title from "./SectionTitle.vue";
import instagramIcon from "../assets/instagram.png";
</script>

<script>
export default {
  data: () => ({
    instagramIcon,
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
      Em 2022, nossa campanha #ProgressNotPerfection IWD alcançou mais de 132
      mil participantes em todo o mundo. Em 2023, nosso objetivo é superar este
      número!
    </p>
    <p class="content">
      Siga nossas redes sociais para informações dos eventos que virão!
    </p>

    <div class="text-center">
      <img height="50" :src="instagramIcon" />
      <h4 class="url" @click="goTo('https://www.instagram.com/iwdsudeste/')">
        @iwdsudeste
      </h4>
    </div>
  </section>
</template>

<style scoped>
.content {
  font-size: 1.1rem;
}
.url {
  margin-top: 10px;
  color: var(--vt-c-blue);
  cursor: pointer;
}
</style>
