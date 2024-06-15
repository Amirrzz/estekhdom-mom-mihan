<template>
  <v-app>
    <Navbar></Navbar>
    <v-main>
      <SectionOne />
      <SectionTwo />
      <SectionThree />
    </v-main>
  </v-app>
</template>

<script setup>
import Navbar from "@/components/navbar.vue";
import SectionOne from "@/components/seciton-one/index.vue";
import SectionTwo from "@/components/section-two/index.vue";
import SectionThree from "@/components/section-three/index.vue";
//
</script>
