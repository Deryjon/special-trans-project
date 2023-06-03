<template>
  <div class="home-page">
    <HeroSection />
  </div>
</template>
<script>
import TheButton from "../../ui/the-button.vue";
import TheTitle from "../../ui/theTitle.vue";
import HeroSection from "../HomePage/sections/HeroSection.vue";

export default { components: { TheButton, TheTitle, HeroSection } };
</script>
