<template>
  <div>
    <v-card class="mx-auto" rounded="lg" variant="text">
      <v-text-field
        placeholder="Your email"
        variant="outlined"
        class="rounded-input"
      ></v-text-field>

      <v-text-field
        :type="visible ? 'text' : 'password'"
        variant="outlined"
        @click:append-inner="visible = !visible"
        placeholder="Your password"
        class="rounded-input"
      ></v-text-field>

      <v-btn
        class="py-6 text-white"
        color="#25DAC5"
        size="large"
        block
        rounded="xl"
        variant="flat"
      >
        Log In
      </v-btn>
      <div class="line">
        <div class="line-item"></div>
        <div class="text">or</div>
        <div class="line-item"></div>
      </div>
      <v-btn
        variant="flat"
        class="py-6 text-white"
        color="#1DA1F2"
        size="large"
        block
        rounded="xl"
      >
        Login via Twitter
      </v-btn>
    </v-card>
  </div>
</template>
<script setup>
import { ref } from "vue";
const visible = ref(null);
</script>
<style scoped>
.line {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 10px;
  margin: 30px 0;
}
.line-item {
  height: 1px;
  background-color: #c5baba;
  width: 50%;
}
</style>
<style>
.rounded-input.v-input .v-field__outline {
  border-radius: 25px;
  --v-field-border-width: 0 !important;
  --v-field-border-opacity: 0;
  border: 1px solid gray;
}
</style>
