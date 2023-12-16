<template>
  <NavBar />
  <FirstScreen />
  <About />
  <Map />
  <Mission />
  <Business />

  <Compensation />

  <Slider />
</template>

<script setup>
import About from "./components/About/About.vue";
import Business from "./components/Business/Business.vue";
import Compensation from "./components/Compensation/Compensation.vue";
import FirstScreen from "./components/FirstScreen/FirstScreen.vue";
import Map from "./components/Map/Map.vue";
import Mission from "./components/Mission/Mission.vue";
import NavBar from "./components/NavBar/NavBar.vue";

import Slider from "./components/Slider/Slider.vue";
</script>
