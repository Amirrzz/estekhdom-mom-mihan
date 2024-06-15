<template>
  <section class="section">
    <v-container class="fill-height flex-column">
      <div class="headers-container">
        <header>
          <span>Plans & Pricing</span>
        </header>
        <div class="sub-header">
          Startup Framework is free forever — you only pay for custom domain
          hosting or to export your site.
        </div>
      </div>
      <v-row class="justify-center prices">
        <v-col cols="12" sm="4">
          <PriceCard plan="starter" />
        </v-col>
        <v-col cols="12" sm="4"
          ><PriceCard plan="professional" :recommended="true"
        /></v-col>
        <v-col cols="12" sm="4"><PriceCard plan="team" /></v-col>
      </v-row>
    </v-container>
  </section>
</template>
<script setup>
import PriceCard from "@/components/section-four/price-card.vue";
</script>
<style scoped>
.section {
  background-image: linear-gradient(0deg, #2f189380, #2f189380),
    url("@/assets/section-four/section-four-background-image.jfif");
}
.headers-container {
  max-width: 586px;
  text-align: center;
}
header {
  font-size: 42px;
}
.sub-header {
  margin-top: 20px;
  margin-bottom: 50px;
  font-size: 22px;
}
</style>
