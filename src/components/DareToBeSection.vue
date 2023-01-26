<template>
  <section>
    <Title text="#DareToBe" />
    <v-row style="width: 100vw" justify="center" align="center">
      <v-col cols="12" lg="6" md="6" sm="6" xs="12">
        <v-img :src="dareToBeSticker" class="align-end" height="200px"> </v-img>
      </v-col>
      <v-col cols="12" lg="6" md="6" sm="6" xs="12">
        <v-card flat>
          <v-row justify="center">
            <v-col cols="9">
              <p class="content">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut
                enim ad minim veniam, quis nostrud exercitation ullamco laboris
                nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor
                in reprehenderit in voluptate velit esse cillum dolore eu fugiat
                nulla pariatur. Excepteur sint occaecat cupidatat non proident,
                sunt in culpa qui officia deserunt mollit anim id est laborum.
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
@media (max-width: 600px) {
  .content {
    text-align: center;
  }
}
@media (min-width: 601px) {
  .content {
    text-align: end;
  }
}

section {
  gap: 32px;
}

.content {
  font-size: 1.1rem;
}
</style>
