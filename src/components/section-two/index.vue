<template>
  <section class="section-one">
    <v-container class="fill-height">
      <v-row class="justify-center ga-6">
        <v-col cols="12" md="5">A</v-col>
        <v-col cols="12" md="5">A</v-col>
      </v-row>
    </v-container>
  </section>
</template>
<script setup>
import Slider from "@/components/seciton-one/slider.vue";
</script>
<style scoped>
.section-one {
  background: linear-gradient(0deg, #2f189380, #2f189380),
    url("@/assets/section-two/section-two-background-image.jfif");
  height: 100%;
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
}
</style>
