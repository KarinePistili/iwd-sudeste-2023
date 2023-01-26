<template>
  <div>
    <v-row style="width: 100vw" justify="center">
      <v-col cols="12" lg="3" md="4" sm="6" xs="12">
        <v-card width="100%" class="px-5" flat>
          <v-img
            :src="sticker"
            alt="Social Gif IWD 2023"
            class="align-end"
            height="200px"
          >
          </v-img>
        </v-card>
      </v-col>
    </v-row>

    <v-footer class="bg-black text-center d-flex flex-column mt-4">
      <!-- <v-btn
        v-for="icon in icons"
        :key="icon"
        class="mx-4"
        :icon="icon"
        variant="plain"
        size="small"
      ></v-btn> -->
      <div>{{ new Date().getFullYear() }} — <strong>IWD Sudeste</strong></div>
    </v-footer>
  </div>
</template>

<script setup>
import sticker from "../assets/sticker-event.gif";
</script>

<script>
export default {
  data: () => ({
    sticker,
     icons: [
        'mdi-facebook',
        'mdi-twitter',
        'mdi-linkedin',
        'mdi-instagram',
      ],
  }),
};
</script>
