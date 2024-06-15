<template>
  <div class="content-container mx-auto align-md-end">
    <div class="pa-8 main-container">
      <header>Let’s Keep in Touch</header>
      <p class="">
        We have created a new product that will help designers, developers and
        companies create websites for their startups quickly and easily.
      </p>
      <a class="row-item" href="tell:+1 555 505 5050">
        <span> <v-icon icon="fa-phone" /> </span>
        <span>+1 555 505 5050</span>
      </a>
      <a class="row-item" href="mailto:info@designmodo.com">
        <span> <v-icon icon="fa-envelope" /> </span>
        <span>info@designmodo.com</span>
      </a>
      <div class="row-item">
        <span> <v-icon icon="fa-building-o" /> </span>
        <span
          >San Francisco, CA560 Bush St & 20th Ave, Apt5 San Francisco,
          230909</span
        >
      </div>
    </div>
  </div>
</template>
<style scoped>
.content-container {
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
  height: 100%;
  padding: 0 100px;
  font-weight: bold;
  align-items: center;
}
.main-container {
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
  height: 100%;
  gap: 24px;
  max-width: 420px;
}
header {
  font-size: 42px;
  max-width: 370px;
}
p {
  font-size: 16px;
  max-width: 370px;
}
a {
  text-decoration: none;
  color: white;
}

.row-item {
  display: flex;
  justify-content: flex-start;
  align-items: baseline;
  gap: 14px;
}
</style>
