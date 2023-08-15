<template>
  <div class="about-us-page">
    <div class="about-square">
      <h4>Vem är jag och vad<br>kan du förvänta dig?</h4>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nisi, hic adipisci illo aperiam praesentium repudiandae officia saepe inventore obcaecati quo!</p>
    </div>
    <div class="matte-container">
      <img src="matte.png" alt="Picture of coach">
      <!-- <img :src="matteImage" alt="Picture of coach"> -->
    </div>
  </div>
</template>

<script setup>
  // import { ref } from 'vue'
  // const matteImage = ref("")
  // matteImage = `${process.env.BASE_URL}matte.png` NÅNTING ATT FIXA SEN VID BUILD
</script>

<style scoped>
  .about-us-page {
    position: relative;
  }
</style>
