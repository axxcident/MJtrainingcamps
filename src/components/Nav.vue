<template>
  <div class="welcome-page" >
    <h1 class="header-text" @click="toggleWelcomeText" >MJ TRAINING CAMP</h1>
    <div class="navigation-meny">
      <button @click="toggleWelcomeText" >
        <h4 class="meny-val">Om Oss</h4>
      </button>
      <button @click="toggleWelcomeText" >
        <h4 class="meny-val">Träningsanläggningen</h4>
      </button>
      <button @click="toggleWelcomeText" >
        <h4 class="meny-val">Phuket</h4>
      </button>
      <button @click="toggleWelcomeText" >
        <h4 class="meny-val">Boka</h4>
      </button>
    </div>
  </div>
  <yellowPlank v-if="welcomeText" />
  <AboutUs v-if="AboutUsText" />
</template>

<script setup>
import yellowPlank from './yellowPlank.vue'
import AboutUs from './AboutUs.vue';

import { ref } from 'vue'
const welcomeText = ref(true)
const AboutUsText = ref(false)
const toggleWelcomeText = () => {
  welcomeText.value = !welcomeText.value;
  AboutUsText.value = !AboutUsText.value;
}

    // <p>hej</p>
    // <p>{{count}}</p>
    // <button @click="count++">Increment Count</button>
    // <p>{{ myData }}</p>
    // <p>{{ reversedData }}</p>
    // <button @click="myData = 'Updated Data'" >Update Data</button>
    // <p>{{ message }}</p>
// import { ref, computed } from 'vue'
// const props = defineProps({
//   message: String,
// })
// const myData = ref('Initial Value')
// const reversedData = computed(() => myData.value.split('').reverse().join(''))
// const count = ref(0)

</script>

<style scoped>

.welcome-page {
  max-width: 1280px;
  margin: 0 auto;
  padding: 2rem;
  text-align: center;
}

</style>
