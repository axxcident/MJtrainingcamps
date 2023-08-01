<template>
  <div class="page-1">
    <div class="welcome-info">
      <div class="welcome-info-flex">
        <h4 class="welcome-info-text">hej</h4>
        <h4 class="welcome-info-text">hej</h4>
        <h4 class="welcome-info-text">hej</h4>
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
    width: 600px;
  }
  .welcome-info {
    z-index: 1;
    position: absolute;
    bottom: 4em;
    left: 20em;
  }
</style>
