<template>
  <section class="delivery ">
    <div class="wrapper xl:flex ">
      <div class="container lg:w-[720px] lg:ml-6">
        <TheTitle>Доставка</TheTitle>
        <p
          class="text-sm lg:text-xl text-[#67675F] lg:text-[#1E1E1C] lg:w-[579px] leading-5 mt-6 font-normal mb-6"
        >
          Основная миссия компании Спец-транс — комплексные поставки нерудных
          материалов для корпоративных клиентов и частных лиц. Мы осуществлем
          доставку по Санкт-Петербургу и Ленинградской области.
        </p>
        <DeliveryService
          class="mb-20"
          v-for="item in deliveryServicesData"
          :key="item.name"
          :data="item"
        />
        <div class="loc lg:mt-[178px] lg:flex lg:gap-5 items-center mb-8">
          <div
            class="location w-full lg:w-[340px] h-[100px] lg:h-[200px] bg-[#F8F8F8]"
          >
            <p class="pt-5 pl-[75px] text-lg font-medium lg:pt-[71px]">
              г. Санкт-Петербург,
            </p>
            <p class="pt-5 pl-[67px] text-base text-[#848692]">
              Невский проспект, д. 12/2
            </p>
          </div>
          <div
            class="location w-full lg:w-[340px] h-[100px] lg:h-[200px] bg-[#F8F8F8] mt-[15px] lg:mt-[0px]"
          >
            <p class="pt-5 pl-[93px] text-lg font-medium lg:pt-[71px]">
              +7 812 545 44 53
            </p>
            <p class="pt-5 pl-[57px] text-base text-[#848692]">
              Ежедневно с 08:00 до 24:00
            </p>
          </div>
        </div>
      </div>
      <div class="img-location lg:w-[1024px] lg:h-[980px]">
        <img
          class="absolute m-12 lg:m-[120px]  lg:w-[600px] lg:h-[600px]"
          src="../../../assets/icons/circle.svg"
          alt=""
        />
        <img
          class="w-[400px] lg:w-full h-[387px] lg:h-full lg:object-cover"
          src="../../../assets/images/location.jpg"
          alt=""
        />
      </div>
    </div>
  </section>
</template>
<script>
import TheTitle from "../../../ui/theTitle.vue";
import DeliveryService from "../components/DeliveryCard.vue";

export default {
  components: { TheTitle, DeliveryService },
  data() {
    return {
      deliveryServicesData: [
        {
          image: "src/assets/icons/star.svg",
          name: "Вы оставляете заявку через сайт или по телефону.",
        },
        {
          image: "src/assets/icons/star.svg",
          name: "Мы производим точный расчет стоимости",
        },
        {
          image: "src/assets/icons/star.svg",
          name: "Осуществляем поставку заказанного вами материала точно в срок",
        },
        {
          image: "src/assets/icons/star.svg",
          name: "Соблюдаем своевременный документообороти",
        },
      ],
    };
  },
};
</script>
