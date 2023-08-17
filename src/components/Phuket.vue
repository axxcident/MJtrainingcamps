<template>
  <div class="google-maps-container">
    <div class="above-map">
      <div class="white-line-1"></div>
      <h3>Här är MJ Training Camp</h3>
      <div class="white-line-2"></div>
    </div>
    <div class="image-map-container">
      <a :href=externalLink target="_blank">
        <img src="/kartan6.png" alt="Map of training camp in Phuket">
      </a>
    </div>
    <h3 class="below-map">Här finns vi: Ratsada, Mueang Phuket District, Phuket, Thailand </h3>
  </div>
</template>

<script setup>
  const externalLink = "https://www.google.com/maps/place/7%C2%B054'42.6%22N+98%C2%B020'11.7%22E/@7.9024802,98.338406,12z/data=!4m13!1m8!3m7!1s0x30503223b80a46f5:0x40223bc2c382420!2sRatsada,+Mueang+Phuket+District,+Phuket,+Thailand!3b1!8m2!3d7.9056936!4d98.3677009!16s%2Fg%2F1v3_02z3!3m3!8m2!3d7.9118333!4d98.3365833?entry=ttu"
</script>

<style scoped>
  .google-maps-container {
    display: flex;
    flex-direction: column;
    margin: 70px auto;
    width: 70%;
    background-color: rgba(0, 0, 0, 0.3);
    border-radius: 52px;
  }

  .above-map {
    max-width: 60vw;
    display: flex;
    margin: 0 auto;
  }

  .above-map h3 {
    font-family: 'Inika', serif;
    color: rgb(255, 255, 255);
    text-shadow: 2px 2px 3px black;
    font-size: 36px;
  }

  .white-line-1 {
    width: 212px;
    height: 2px;
    margin-top: 25px;
    background-color: white;
    margin-right: 15px;
  }
  .white-line-2 {
    width: 212px;
    height: 2px;
    margin-top: 25px;
    background-color: white;
    margin-left: 15px;
  }

  .below-map {
    font-family: 'Inika', serif;
    color: rgb(255, 255, 255);
    text-shadow: 2px 2px 3px black;
    font-size: 30px;
    text-align: center;
  }

  .image-map-container {
    max-width: 60vw;
    display: flex;
    margin: 0 auto;
  }

  .image-map-container a img {
    width: 100%;
    cursor: pointer;
  }
</style>
