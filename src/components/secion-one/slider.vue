<template>
  <v-carousel height="400" hide-delimiter-background show-arrows>
    <template v-slot:prev="{ props }">
      <v-icon icon="fa-angle-left" @click="props.onClick" />
    </template>
    <template v-slot:next="{ props }">
      <v-icon icon="fa-angle-right" @click="props.onClick" />
    </template>
    <template v-slot:delimiter:="{ props }"> {{ props }} </template>
    <v-carousel-item v-for="(slide, i) in 5" :key="i">
      <div class="slide-item text-center">
        <div class="subheadr">Startup 3</div>
        <div class="header">Forget About Code</div>
        <div class="discription">
          Startup Framework gives you complete freedom over your creative
          process — you don’t have to think about any technical aspects. There
          are no limits and absolutely no coding.
        </div>
      </div>
    </v-carousel-item>
  </v-carousel>
</template>
<style scoped>
.slide-item {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 28px;
  max-width: 736px;
  margin: auto;
}
.subheadr {
  font-size: 24px;
}
.header {
  font-size: 72px;
}
.discription {
  font-size: 22px;
}
</style>
<style>
.v-carousel .fa-circle:before {
  content: "";
  height: 10px;
  width: 10px;
  border-radius: 50%;
  border: 2px solid white;
}
.v-carousel .v-btn--active .fa-circle:before {
  background-color: white;
}
</style>
