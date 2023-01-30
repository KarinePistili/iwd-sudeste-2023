<template>
  <section class="mt-14">
    <Title text="#DareToBe" />
    <v-row style="width: 100%" justify="center" align="center">
      <v-col cols="12" lg="6" md="6" sm="6" xs="12">
        <v-img :src="dareToBeSticker" class="align-end" height="200px"> </v-img>
      </v-col>
      <v-col cols="12" lg="6" md="6" sm="6" xs="12">
        <v-card flat>
          <v-row justify="center">
            <v-col>
              <p class="content">
                No Dia Internacional das Mulheres, celebramos as mulheres que
                ousam ser fortes, resilientes e inovadoras. Essas que são
                exemplos de coragem e determinação, que enfrentam desafios e
                superam obstáculos diários para alcançar seus objetivos e
                realizar seus sonhos.
              </p>
              <p class="content">
                Ainda que tudo pareça impossível, mulheres tem a Força para se
                levantar quando caem, são Resilientes para persistirem lutando,
                e são Inovadoras e capazes de encontrar esperança e
                oportunidades mesmo em meio à adversidade. Qualidades essas que
                são essenciais para um mundo onde ainda enfrentamos muitas
                desigualdades e barreiras.
              </p>
              <p class="content">
                Mulheres ao "ousarem ser" mostram ao mundo que vencem qualquer
                desafio. Assim como Ada Lovelace, Grace Hopper, Katherine
                Johnson, Roberta Andrade, e muitas outras. Vamos continuar a
                celebrar as mulheres #daretobe e inspirar as próximas gerações a
                seguir seus exemplos e construir novos caminhos.
              </p>
              <p class="content">
                <strong>Juntas, transformamos tudo.</strong>
              </p>
            </v-col>
          </v-row>
        </v-card>
      </v-col>
    </v-row>
  </section>
</template>

<script setup>
import dareToBeSticker from "../assets/sticker-dare-to-be.gif";
import Title from "./SectionTitle.vue";
</script>

<script>
export default {
  data: () => ({
    dareToBeSticker,
  }),
  components: {
    Title,
  },
};
</script>

<style scoped>
@media (max-width: 768px) {
  .content {
    text-align: center;
  }
}

@media (min-width: 769px) {
  section {
    gap: 32px;
  }
}

.content {
  font-size: 1.1rem;
}
</style>
