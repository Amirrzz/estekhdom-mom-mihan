<template>
  <v-card color="white tabs-card mx-auto " max-width="500">
    <v-row class="justify-center px-12 py-16">
      <v-col cols="8">
        <label for="firstName">YOUR NAME</label>
        <v-text-field
          id="firstName"
          placeholder="Your email"
          variant="outlined"
          class="rounded-input"
        ></v-text-field>
      </v-col>
      <v-col cols="4">
        <label for="budget">BUDGET</label>
        <v-select
          v-model="budget"
          :items="[500, 2500, 5000]"
          variant="outlined"
          class="rounded-input"
        ></v-select>
      </v-col>
      <v-col cols="12">
        <label for="inputField">INPUT FIELD</label>
        <v-text-field
          id="inputField"
          placeholder="name@mail.com"
          variant="outlined"
          class="rounded-input"
        ></v-text-field>
      </v-col>
      <v-col cols="12">
        <label for="messageInput">YOUR MESSAGE</label>
        <v-textarea
          id="messageInput"
          placeholder="name@mail.com"
          variant="outlined"
          class="rounded-input"
        ></v-textarea>
      </v-col>
      <v-col cols="12">
        <v-row class="align-center justify-between">
          <v-col cols="6" class="mx-auto">
            <v-checkbox
              v-model="sendACopy"
              color="#25DAC5"
              label="Send me a copy"
              :value="true"
              hide-details
            ></v-checkbox>
          </v-col>
          <v-col cols="6" class="text-right">
            <v-btn
              rounded="xl"
              size="x-large"
              color="#25DAC5"
              variant="flat"
              class="text-white"
              >Send</v-btn
            >
          </v-col>
        </v-row>
      </v-col>
    </v-row>
  </v-card>
</template>
<script setup>
import { ref } from "vue";
const budget = ref(500);
const sendACopy = ref(false);
</script>
<style scoped>
label {
  color: #1e0e62;
  font-size: 14px;
  font-weight: bold;
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
