<script setup>
import Title from "./SectionTitle.vue";
import gCloudLogo from "../assets/google-cloud-logo.png";
import gDevelopersGroupLogo from "../assets/google-developers-logo.jpg";
import oneBitCodeLogo from "../assets/onebitcode-logo.png";
import nearSureLogo from "../assets/nearsure-logo.png";
</script>

<script>
export default {
  data: () => ({
    groups: [
      {
        src: gCloudLogo,
        flex: 3,
      },
      {
        src: gDevelopersGroupLogo,
        flex: 3,
      },
      {
        src: oneBitCodeLogo,
        flex: 3,
      },
      {
        src: oneBitCodeLogo,
        flex: 3,
      },
    ],
  }),
};
</script>

<template>
  <section>
    <Title text="Patrocinadores" />
    <span class="cota">
      <strong>Cota Dare To Be</strong>
    </span>
    <v-row style="width: 100vw" class="pa-12 pt-3" justify="center">
      <v-col cols="12" lg="3" md="4" sm="6" xs="12">
        <v-card width="100%" class="px-5">
          <v-img :src="gCloudLogo" class="align-end" height="200px"> </v-img>
        </v-card>
      </v-col>
      <v-col cols="12" lg="3" md="4" sm="6" xs="12">
        <v-card width="100%" class="px-5">
          <v-img :src="gDevelopersGroupLogo" class="align-end" height="200px">
          </v-img>
        </v-card>
      </v-col>
    </v-row>
    <span class="cota">
      <strong>Cota Innovative</strong>
    </span>
    <v-row style="width: 100vw" class="pa-12 pt-3" justify="center">
      <v-col cols="12" lg="3" md="4" sm="6" xs="12">
        <v-card width="100%" class="px-5">
          <v-img :src="oneBitCodeLogo" class="align-end" height="200px"> </v-img>
        </v-card>
      </v-col>
    </v-row>
    <span class="cota">
      <strong>Cota Bold</strong>
    </span>
    <v-row style="width: 100vw" class="pa-12 pt-3" justify="center">
      <v-col cols="12" lg="3" md="4" sm="6" xs="12">
        <v-card width="100%" class="px-5">
          <v-img :src="nearSureLogo" class="align-end" height="200px"> </v-img>
        </v-card>
      </v-col>
    </v-row>
  </section>
</template>

<style scoped>
section {
  margin-top: 60px;
}

.cota {
  font-size: 1.5rem;
  color: var(--vt-c-blue);
}
</style>
