<template>
  <div class="welcome-page" >
    <h1 class="header-text" @click="toggleWelcomeText" >MJ TRAINING CAMP</h1>
    <div class="navigation-meny">
      <button @click="toggleAboutUsText" >
        <h4 :class="{ active: AboutUsText }" class="meny-val">Om Oss</h4>
      </button>
      <button @click="toggleLocationText" >
        <h4 :class="{ active: LocationText }" class="meny-val">Träningsanläggningen</h4>
      </button>
      <button @click="togglePhuketText" >
        <h4 :class="{ active: PhuketText }" class="meny-val">Phuket</h4>
      </button>
      <button @click="toggleBookingText" >
        <h4 :class="{ active: BookingText }" class="meny-val">Boka</h4>
      </button>
    </div>
  </div>
  <yellowPlank v-if="welcomeText" />
  <AboutUs v-if="AboutUsText" />
  <Location v-if="LocationText" />
  <Phuket v-if="PhuketText" />
  <Booking v-if="BookingText" />
</template>

<script setup>
import yellowPlank from './yellowPlank.vue'
import AboutUs from './AboutUs.vue';
import Location from './Location.vue';
import Phuket from './Phuket.vue';
import Booking from './Booking.vue'

import { ref } from 'vue'
const welcomeText = ref(true)
const AboutUsText = ref(false)
const LocationText = ref(false)
const PhuketText = ref(false)
const BookingText = ref(false)

const toggleWelcomeText = () => {
  welcomeText.value = true;
  AboutUsText.value = false;
  LocationText.value = false;
  PhuketText.value = false;
  BookingText.value = false;
}
const toggleAboutUsText = () => {
  welcomeText.value = false;
  AboutUsText.value = true;
  LocationText.value = false;
  PhuketText.value = false;
  BookingText.value = false;
}
const toggleLocationText = () => {
  welcomeText.value = false;
  AboutUsText.value = false;
  LocationText.value = true;
  PhuketText.value = false;
  BookingText.value = false;
}
const togglePhuketText = () => {
  welcomeText.value = false;
  AboutUsText.value = false;
  LocationText.value = false;
  PhuketText.value = true;
  BookingText.value = false;
}
const toggleBookingText = () => {
  welcomeText.value = false;
  AboutUsText.value = false;
  LocationText.value = false;
  PhuketText.value = false;
  BookingText.value = true;
}

</script>

<style scoped>

.welcome-page {
  max-width: 1280px;
  margin: 0 auto;
  padding: 2rem;
  text-align: center;
}

.active {
  text-decoration: underline;
  font-size: 1.5em !important;
}

</style>
