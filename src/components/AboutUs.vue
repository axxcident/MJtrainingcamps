<template>
  <div class="about-us-page">
    <div class="about-square">
      <h4>Vem är jag och vad kan du förvänta dig?</h4>
      <p>Hej jag heter Mathias Jonsson Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore</p>
    </div>
    <div class="matte-container">
      <img src="matteb.png" alt="Picture of coach">
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

  .matte-container {
    position: fixed;
    right: -7rem;
    bottom: -40rem;
  }

  .about-square {
    width: 437px;
    height: 761px;
    background-color: #FFD119;
    border-radius: 67px;

    position: fixed;
    left: 13rem;
    bottom: -14rem;

    display: flex;
    flex-direction: column;
  }

  @media (max-width: 1500px) {
    .about-square {
      left: 5rem;
    }
  }
  @media (max-width: 1280px) {
    .about-square {
      width: 400px;
      height: 651px;
    }

    .about-square h4, p {
      width: 361px !important;
    }

    .about-square h4 {
      font-size: 26px !important;
    }
    .about-square p {
    font-size: 16px !important;
    }
    .matte-container {
      right: -13rem;
    }
    .matte-container img {
      width: 85vw;
      min-width: 1028px;
    }
  }

  .about-square h4, p {
    font-family: 'Inika', serif;
    width: 400px;
    margin: 10px 19px;
    padding: 2px 16px 0 16px;
  }

  .about-square h4 {
    font-size: 36px;
    font-weight: 500;
  }

  .about-square p {
    font-size: 24px;
  }

</style>
