<script setup>
import { RouterLink } from "vue-router";
import Title from "./SectionTitle.vue";
</script>

<script>
export default {
  methods: {
    goTo(url) {
      window.open(url);
    },
  },
};
</script>

<template>
  <section>
    <Title text="Inscrições Abertas!" />
    <p class="content">
      Estão <strong>ABERTAS AS INSCRIÇÕES</strong> para o IWD Sudeste 2023. Esse evento será
      realizado na <strong>Google São Paulo</strong>, no dia <strong>25/03/2023</strong>, das 13h00min as
      18h00min, em duas modalidades <strong>GRATUITAS</strong>: online e presencial. O presencial
      é <strong>LIMITADO</strong> e <strong>EXCLUSIVO</strong> para mulheres (cis e trans). Por gentileza, só
      adquira o ingresso presencial caso tenha <strong>CERTEZA</strong> de comparecimento no
      evento. Entraremos em contato pelo e-mail <strong>iwdsudeste@gmail.com</strong> As
      inscrições podem ser realizadas através do botão abaixo
    </p>
    <v-row justify="center" class="my-4">
      <div class="btn" @click="goTo('https://www.sympla.com.br/evento/iwd-sudeste-2023/1873998?lang=PT')">
        <h3>Inscreva-se aqui!</h3>
      </div>
    </v-row>
  </section>
</template>

<style scoped>
.btn {
  background: linear-gradient(
    90deg,
    rgba(76, 198, 246, 1) 0%,
    rgba(27, 228, 181, 1) 50%,
    rgba(48, 172, 212, 1) 85%
  );
}
.content {
  font-size: 1.1rem;
}
</style>
