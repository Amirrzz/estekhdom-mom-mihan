<template>
  <v-app>
    <Navbar></Navbar>
    <v-main>
      <SectionOne />
      <SectionTwo />
      <SectionThree />
      <SectionFour />
    </v-main>
    <Footer></Footer>
  </v-app>
</template>

<script setup>
import Navbar from "@/components/navbar.vue";
import SectionOne from "@/components/seciton-one/index.vue";
import SectionTwo from "@/components/section-two/index.vue";
import SectionThree from "@/components/section-three/index.vue";
import SectionFour from "@/components/section-four/index.vue";
import Footer from "@/components/AppFooter.vue";
//
</script>
