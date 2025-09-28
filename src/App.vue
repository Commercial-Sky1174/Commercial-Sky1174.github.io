<script setup>
import { onBeforeUnmount, onMounted, ref } from "vue";
import Navigation from "./components/Navigation.vue";
import Footer from "./components/Footer.vue";

// Vanta
import NET from "vanta/dist/vanta.net.min";
import * as THREE from "three";
import feather from "feather-icons";

const vantaRef = ref(null);
let vantaEffect = null;

onMounted(() => {
  // Initialize Vanta.js background
  vantaEffect = NET({
    el: vantaRef.value,
    THREE,
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

  // Replace feather icons
  feather.replace();

  // Animate progress bar
  const progressBar = document.querySelector(".progress-bar");
  let width = 0;
  const targetWidth = 65;
  const interval = setInterval(() => {
    if (width >= targetWidth) {
      clearInterval(interval);
    } else {
      width++;
      progressBar.style.width = width + "%";
    }
  }, 20);
});

onBeforeUnmount(() => {
  if (vantaEffect) vantaEffect.destroy();
});
</script>

<template>
  <div ref="vantaRef" id="vanta-bg"></div>

  <Navigation />

  <router-view />

  <Footer />
</template>

<style scoped></style>
