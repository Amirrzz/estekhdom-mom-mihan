<template>
  <section class="section">
    <v-container class="fill-height">
      <v-responsive class="align-centerfill-height mx-auto">
        <v-row class="justify-center ga-6">
          <v-col cols="12"><Slider></Slider></v-col>
          <v-col cols="12" md="3" sm="6" class="text-center">
            <v-btn rounded="xl" size="x-large" color="#482BE7" variant="flat"
              >Create an Account</v-btn
            >
          </v-col>
        </v-row>
      </v-responsive>
    </v-container>
  </section>
</template>

<script setup>
import Slider from "@/components/seciton-one/slider.vue";
</script>

<style scoped>
.section {
  background-image: linear-gradient(0deg, #2f189380, #2f189380),
    url("@/assets/section-one/section-one-background-image.jfif");
}
</style>
