<template>
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

  .background-placeholder {
    z-index: 0;
  }

  .welcome-info-flex {
    display: flex;
    justify-content: space-around;
    /* width: 600px; */
  }
  .welcome-info {
    z-index: 1;
    position: absolute;
    width: 78%;
    margin-top: 4%;
    margin-left: 7%;
  }

  .welcome-info-text {
    color: #ffffff;
    text-shadow: 2px 2px 3px black;
    font-size: 1.6em;
    font-weight: 600;
  }
</style>
