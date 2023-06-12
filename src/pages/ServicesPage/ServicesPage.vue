<template>
  <main class="materials-page">
    <ServicesSection />
    <QuestionComponent />
  </main>
</template>
<script>
import QuestionComponent from "../../components/questionComponent.vue";
import ServicesSection from "./sections/ServicesSection.vue";

export default {
  components: { QuestionComponent, ServicesSection },
};
</script>
