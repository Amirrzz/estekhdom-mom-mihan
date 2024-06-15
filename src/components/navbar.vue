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
  position: sticky;
  top: 85px;
  left: 0;
}
a {
  text-decoration: none;
  font-size: 18px;
  line-height: 26px;
  color: white;
  font-weight: 500;
}
.active-link {
  opacity: 30%;
}
</style>
