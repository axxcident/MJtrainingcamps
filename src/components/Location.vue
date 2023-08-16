<template>
  <div class="location-page">
    <div class="location-square">
      <h4>Tränings<br>anläggningen</h4>
      <p>I Phuket på X så har vi många aktiviteter förberedda åt er. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate</p>
    </div>
    <div class="circles-container">
      <img src="BeachGym.jpg" alt="exercise on beach" class="circular-image-1" />
      <!-- <img src="matteb.png" alt="Picture of coach"> -->
    </div>
  </div>
</template>

<script setup>

</script>

<style scoped>
  .location-page {
    position: relative;
  }

  .circles-container {
    position: fixed;
    left: 756px;
    top: 560px;

    width: 235px; /* Adjust the width and height as needed */
    height: 235px;
    overflow: hidden;
    border-radius: 50%;
  }

  .circular-image-1 {
    width: 100%;
    height: 100%;
    object-fit: cover;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}

  .location-square {
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

  .location-square h4, p {
    font-family: 'Inika', serif;
    width: 400px;
    margin: 10px 19px;
    padding: 2px 16px 0 16px;
  }

  .location-square h4 {
    text-align: center;
    font-size: 36px;
    font-weight: 500;
  }

  .location-square p {
    font-size: 24px;
  }

</style>
