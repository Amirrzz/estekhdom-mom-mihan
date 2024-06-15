<template>
  <nav>
    <a href="#" class="active-link">Home</a>
    <a href="#">Features</a>
    <a href="#">Pricing</a>
    <a href="#">Blog</a>
    <a href="#"> <v-icon icon="fa-dribbble" /> </a>
    <a href="#"> <v-icon icon="fa-behance" /> </a>
  </nav>
</template>
<style scoped>
nav {
  display: flex;
  justify-content: center;
  gap: 4%;
  position: absolute;
  top: 85px;
  width: 100%;
  left: 0;
}
a {
  font-size: 18px;
}
.active-link {
  opacity: 30%;
}
</style>
