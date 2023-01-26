<script setup>
import Title from "./SectionTitle.vue";
import gCloudLogo from "../assets/google-cloud-logo.png"
</script>

<script>
export default {
  data: () => ({
    groups: [
      {
        src: gCloudLogo,
        flex: 3,
      },
    ],
  }),
};
</script>

<template>
  <section>
    <Title text="Patrocinadores" />
     <v-row style="width: 100vw" class="pa-12" justify="center">
      <v-col cols="12" lg="3" md="4" sm="6" xs="12">
        <v-card width="100%" class="px-5">
          <v-img :src="gCloudLogo" class="align-end" height="200px"> </v-img>
        </v-card>
      </v-col>
    </v-row>
    <!-- <div class="sponsors">
      <img src="@/assets/sponsors.png" />
      <img src="@/assets/sponsors.png" />
      <img src="@/assets/sponsors.png" />
      <img src="@/assets/sponsors.png" />
      <img src="@/assets/sponsors.png" />
      <img src="@/assets/sponsors.png" />
    </div> -->
  </section>
</template>

<style scoped>
section {
  margin-top: 0;
}
.sponsors {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-gap: 24px;
}
</style>
