<template>
  <div class="bubble-container">
    <img src="../assets/yellowBubble.svg" alt="yellow ellipse">
    <div class="bubble-text-container">
      <p>DEL I<br>DUBBELRUM<br>21990:-</p>
      <p>ENKELRUM<br>23990:-</p>
    </div>
  </div>
  <div class="page-1">
    <div class="welcome-info">
      <div class="welcome-info-flex">
        <h4 class="welcome-info-text">2 Träningspass<br>dagligen</h4>
        <h4 class="welcome-info-text">Bo i hotel nära<br>stranden</h4>
        <h4 class="welcome-info-text">Flyg tur/retur<br>1/12-11/12</h4>
      </div>
    </div>
    <img src="../assets/yellowPlank.svg" class="background-placeholder" alt="background placeholder" />
  </div>
</template>

<script setup>
// Vue script
</script>

<style scoped>

  .bubble-container {
    position: relative;
  }

  .bubble-container img {
    position: absolute;
    right: 25px;
    top: 9rem;
    z-index: 1;
  }

  .bubble-text-container {
    height: 210px;
    position: absolute;
    right: 80px;
    top: 10rem;
    z-index: 2;
    display: flex;
    flex-direction: column;
    /* justify-content: space-around; */

  }

  .bubble-text-container p {
    text-align: center;
    margin: 21px auto;
    font-weight: 600;
    font-family: 'Inter', sans-serif;
  }

  .page-1 {
    /* position:relative; */
    font-family: 'Inika', serif;
  }

  .background-placeholder {
    z-index: 0;
  }

  .welcome-info-flex {
    display: flex;
    justify-content: space-around;
    max-width: 93%;
    margin: 0px 60px;
    /* ÖKA MARGIN STÖRRE ÄN 1650px width */
    /* MINSKA TEXT MINDRE ÄN 1000px width */
  }
  .welcome-info {
    z-index: 1;
    position: absolute;
    width: 78%;
    margin-top: 4%;
    margin-left: 7%;
  }

  @media (min-width: 1500px) {
    .welcome-info {
      margin-top: 3%;
    }
  }

  .welcome-info-text {
    color: #ffffff;
    text-shadow: 2px 2px 3px black;
    font-size: 1.6em;
    font-weight: 600;
    text-align: center;
  }

  @media (max-width: 1100px) {
    .welcome-info-text {
      font-size: 1.4em;
    }
  }
  @media (max-width: 860px) {
    .welcome-info-text {
      font-size: 1.2em;
    }
  }
  @media (max-width: 700px) {
    .welcome-info-text {
      font-size: 1em;
    }
  }


</style>
