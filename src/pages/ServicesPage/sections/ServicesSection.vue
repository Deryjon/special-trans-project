<template>
  <section class="services min-h-screen lg:mt-48">
    <div class="container">
      <ServicesCard
        v-for="item in servicesData"
        :key="item.title"
        :data="item"
      />
    </div>
  </section>
</template>
<script>
import ServicesCard from "../components/ServicesCard.vue";

export default {
  data() {
    return {
      servicesData: [
        {
          image: "src/assets/images/hero-bg.jpg",
          title: "Аренда спецтехники",
          descprition:
            "Мы перелагаем доступные условия аренды различной техники посуточно и на длительный срок. ",
          price1: "1300 ₽",
          price2: "1500 ₽",
          price3: "2000 ₽",
        },
        {
          image: "src/assets/images/services-1.jpg",
          title: "Аренда самосвалов",
          descprition:
            "Мы перелагаем доступные условия аренды различной техники посуточно и на длительный срок. ",
          price1: "1500 ₽",
          price2: "1500 ₽",
          price3: "1600 ₽",
        },
      ],
    };
  },
  components: { ServicesCard },
};
</script>
