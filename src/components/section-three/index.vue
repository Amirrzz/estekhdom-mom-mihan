<template>
  <section class="section">
    <v-container class="fill-height">
      <v-row class="justify-center">
        <v-col cols="12" md="6"><Content /></v-col>
        <v-col cols="12" md="6"><Signin /></v-col>
      </v-row>
    </v-container>
  </section>
</template>
<script setup>
import Signin from "@/components/section-three/sign-in.vue";
import Content from "@/components/section-three/content.vue";
</script>
<style scoped>
.section {
  background-image: linear-gradient(0deg, #2f189380, #2f189380),
    url("@/assets/section-three/section-three-background-image.jfif");
}
</style>
