<template>
  <main class="materials-page">
    <MaterialsSection/>
    <QuestionComponent />
  </main>
</template>
<script>
import QuestionComponent from "../../components/questionComponent.vue";
import MaterialsSection from "./sections/MaterialsSection.vue";

export default {
  components: { QuestionComponent, MaterialsSection },
};
</script>
