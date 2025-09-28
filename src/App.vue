<script setup>
import { onMounted, ref } from "vue";
import Navigation from "./components/Navigation.vue";
import Footer from "./components/Footer.vue";

const vanta = ref(null);

onMounted(() => {
  // Initialize Vanta.js background
  console.log(vanta.value)
  VANTA.NET({
    el: vanta.value,
    mouseControls: true,
    touchControls: true,
    gyroControls: false,
    minHeight: 200.0,
    minWidth: 200.0,
    scale: 1.0,
    scaleMobile: 1.0,
    color: 0x00ff9d,
    backgroundColor: 0x242424,
    points: 12.0,
    maxDistance: 22.0,
    spacing: 18.0,
  });
});
</script>

<template>
  <div ref="vanta" id="vanta-bg"></div>

  <Navigation />

  <router-view />

  <Footer />
</template>

<style scoped></style>
