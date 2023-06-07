<template>
  <div class="home-page">
    <HeroSection />
    <ServicesSection />
  </div>
</template>
<script>
import HeroSection from "../HomePage/sections/HeroSection.vue";
import ServicesSection from "./sections/ServicesSection.vue";

export default {
  components: {  HeroSection, ServicesSection },
};
</script>
