<script setup>
import { CCarousel, CCarouselItem } from "@coreui/vue";
import Title from "./SectionTitle.vue";
</script>

<template>
  <section class="mt-14">
    <Title text="Palestrantes" />

    <CCarousel controls transition="crossfade">
      <CCarouselItem>
        <div class="d-flex justify-content-center">
          <img
            class="w-50"
            src="@/assets/speakers/GiseliAnversa-Site.jpg"
            alt="Giseli Anversa"
          />
        </div>
      </CCarouselItem>
      <CCarouselItem>
        <div class="d-flex justify-content-center">
          <img
            class="w-50"
            src="@/assets/speakers/GrazielleSilvaRibeiro-Site.jpg"
            alt="Grazielle Silva Ribeiro"
          />
        </div>
      </CCarouselItem>
      <CCarouselItem>
        <div class="d-flex justify-content-center">
          <img
            class="w-50"
            src="@/assets/speakers/JessicaFernandesdeOliveira-Site.jpg"
            alt="Jessica Fernandes de Oliveira"
          />
        </div>
      </CCarouselItem>
      <CCarouselItem>
        <div class="d-flex justify-content-center">
          <img
            class="w-50"
            src="@/assets/speakers/MarianaFilleti-Site.jpg"
            alt="Mariana Filleti"
          />
        </div>
      </CCarouselItem>
      <CCarouselItem>
        <div class="d-flex justify-content-center">
          <img
            class="w-50"
            src="@/assets/speakers/DanielleTorres-Site.jpg"
            alt="Danielle Torres"
          />
        </div>
      </CCarouselItem>
      <CCarouselItem>
        <div class="d-flex justify-content-center">
          <img
            class="w-50"
            src="@/assets/speakers/RobertaLingnaudeOliveira-Site.jpg"
            alt="Roberta Lingnau de Oliveira"
          />
        </div>
      </CCarouselItem>
    </CCarousel>
  </section>
</template>

<style>
.carousel-control-prev-icon {
  background-image: url(@/assets/arrow-left.svg) !important;
}

.carousel-control-next-icon {
  background-image: url(@/assets/arrow-right.svg) !important;
}

.carousel {
  width: 343.2px !important;
}

span {
  font-size: 1.2rem;
  font-weight: 500;
}

@media (min-width: 769px) {
  .carousel {
    width: 450px !important;
  }

  span {
    margin-top: 20px;
  }
}
</style>
