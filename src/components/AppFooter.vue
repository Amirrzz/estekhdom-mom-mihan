<template>
  <v-footer>
    <v-row class="top-part-container">
      <v-col cols="12" md="4"> <div class="brand-name">Startup 3</div> </v-col>
      <v-col cols="12" md="8">
        <div class="options-container">
          <span>Privacy Policy</span>
          <span>Terms</span>
          <v-icon icon="fa-twitter" color="white" size="x-small"></v-icon>
          <v-icon
            icon="fa-facebook-square"
            color="white"
            size="x-small"
          ></v-icon>
          <v-icon
            icon="fa-google-plus"
            color="white"
            size="x-small"
          ></v-icon></div
      ></v-col>
    </v-row>
    <div class="line"></div>
    <v-row class="bottom-part-container">
      <v-col cols="12" md="8">
        <nav class="nav-links">
          <a href="#" class="active-link">Tour</a>
          <a href="#">Features</a>
          <a href="#">Pricing Plans</a>
          <a href="#">Our Works</a>
          <a href="#">Brands</a>
          <a href="#">Contacts</a>
        </nav>
      </v-col>
      <v-col cols="12" md="4">
        <div class="copy-right-content text-right">
          © 2017 Designmodo. All rights reserved.
        </div>
      </v-col>
    </v-row>
  </v-footer>
</template>

<style scoped>
footer {
  background: #2f1893;
  display: flex;
  flex-direction: column;
  padding: 25px 5vw;
}
.brand-name {
  font-size: 24px;
}
.line {
  height: 1px;
  width: 100%;
  background: gray;
  margin: 40px 0;
}
.top-part-container {
  width: 100%;
  margin: unset !important;
  margin-top: 40px;
}
.options-container {
  display: flex;
  justify-content: flex-end;
  gap: 10px;
  align-items: center;
}
.nav-links {
  display: flex;
  justify-content: flex-start;
  gap: 10px;
  align-items: center;
}
.bottom-part-container {
  width: 100%;
  margin: unset !important;
}
</style>
