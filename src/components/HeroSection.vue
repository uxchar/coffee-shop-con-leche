<script setup>
import NavBar from "./NavBar.vue";
</script>
<template>
  <div class="hero-section">
    <NavBar />
    <div class="overlay"></div>
    <video
      class="background-video"
      autoplay
      muted
      loop
      playsinline
      webkit-playsinline
    >
      <source src="/videos/6769796-uhd_3840_2160_24fps.mp4" type="video/mp4" />
    </video>
    <p class="hero-info">
      The finest beans imported from Colombia & Guatemala.
    </p>
  </div>
</template>

<style scoped>
.hero-section {
  display: flex;
  flex-direction: column;
  align-items: center;
  color: #f6f5eb;
  height: 100vh;
  overflow: hidden;
  position: relative;
  background-color: #0e2a54;
}

.background-video {
  width: 100%;
  height: 100%;
  object-fit: cover;
  position: absolute;
  top: 0;
  left: 0;
  z-index: -100;
  visibility: hidden;
}

.overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100vw;
  height: 100vh;
  background: rgba(54, 46, 55, 0.4);
  z-index: -99;
}

.hero-info {
  position: absolute;
  top: 96%;
  left: 50%;
  transform: translate(-50%, -50%);
  white-space: nowrap;
  font-size: 0.7rem;
  z-index: 2;
}

@media screen and (min-width: 1100px) {
  .background-video {
    visibility: visible;
  }
  .hero-section {
    background-color: transparent;
  }
}
</style>
