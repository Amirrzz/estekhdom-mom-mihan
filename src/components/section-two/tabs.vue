<template>
  <v-card color="white tabs-card mx-auto" max-width="500">
    <v-tabs bg-color="white" fixed-tabs v-model="tab">
      <v-tab
        v-for="item in items"
        :key="item"
        :text="item"
        :value="item"
      ></v-tab>
    </v-tabs>
    <v-tabs-window v-model="tab" class="tab-container">
      <v-tabs-window-item v-for="item in items" :key="item" :value="item">
        <v-card flat color="white">
          <SignIn />
        </v-card>
      </v-tabs-window-item>
    </v-tabs-window>
  </v-card>
</template>
<script setup>
import { ref } from "vue";
import SignIn from "@/components/section-two/sign-in.vue";
const tab = ref(null);
const items = ref(["Sign Up", "Log In"]);
const text = ref("text");
</script>
<style scoped>
.tabs-card .v-tabs--density-default {
  --v-tabs-height: 75px;
}
.tab-container {
  padding: 70px;
}
</style>
