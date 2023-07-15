<template>
  <div>
    <p>hej</p>
    <p>{{count}}</p>
    <button @click="count++">Increment Count</button>
    <p>{{ myData }}</p>
    <p>{{ reversedData }}</p>
    <button @click="myData = 'Updated Data'" >Update Data</button>
    <p>{{ message }}</p>
  </div>
</template>

<script setup>
import { ref, computed } from 'vue'
const props = defineProps({
  message: String,
})
const myData = ref('Initial Value')
const reversedData = computed(() => myData.value.split('').reverse().join(''))
const count = ref(0)

</script>

<style scoped>

</style>
