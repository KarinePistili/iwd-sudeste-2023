<template>
  <section class="mt-14">
    <Title text="Call For Papers" />
    <v-row style="width: 100%" justify="center" align="center">
      <v-card flat>
        <v-row justify="center">
          <v-col>
            <p class="content">
              <br />Nosso Call for Papers para o International Women's Day
              Sudeste (IWD) está aberto! Você, mulher, quer ajudar a incentivar
              e promover outras mulheres no mundo da tecnologia? Então submeta
              sua palestra para a gente e nos ajude a fazer com que este IWD
              seja sensacional! As palestras devem ser enviadas até o dia
              <strong style="color: red">10/02</strong>
            </p>
          </v-col>
        </v-row>
      </v-card>
    </v-row>
    <v-row>
      <h5 style="color: red">Submissões encerradas</h5>
      <!-- <v-card
        class="pa-4"
        color="info"
        style="cursor: pointer"
        @click="goTo('https://forms.gle/qkvXoSnxyTw5iVVo7')"
      >
        <h5>Submeta sua proposta</h5>
      </v-card> -->
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
  methods: {
    goTo(url) {
      window.open(url);
    },
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
