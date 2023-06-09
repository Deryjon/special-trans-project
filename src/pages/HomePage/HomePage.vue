<template>
  <div class="home-page">
    <HeroSection />
    <ServicesSection />
    <MainMaterialsSection />
    <AboutSection />
    <QuestionComponent />
  </div>
</template>
<script>
import QuestionComponent from "../../components/questionComponent.vue";
import HeroSection from "../HomePage/sections/HeroSection.vue";
import AboutSection from "./sections/AboutSection.vue";
import MainMaterialsSection from "./sections/MainMaterialsSection.vue";
import ServicesSection from "./sections/ServicesSection.vue";

export default {
  components: {
    HeroSection,
    ServicesSection,
    MainMaterialsSection,
    AboutSection,
    QuestionComponent,
  },
};
</script>
