<template>
  <section class="about mb-16 ">
    <div class="container">
      <div class="wrapper md:flex md:justify-between 2xl:gap-28 xl:gap-0 mr-0 ml-0 lg:flex-wrap lg:wrap  md:ml-0  ">
        <div class="left lg:w-[580px] h-[235px] lg:mt-28 flex flex-col md:mt-16 ">
          <TheTitle>О компании СПЕЦ-ТРАНС</TheTitle>
          <p
            class="w-[335px] h-[160px] lg:w-[580px] text-sm text-[#67675F] font-normal mt-6 lg:mt-[28px]"
          >
            Наша фирма существует уже многие годы, заработав репутацию на рынке
            предлагаемых услуг как надежного и ответственного партнера. В число
            наших клиентов вошли крупнейшие организации. При этом стоит
            отметить, что на индивидуальный подход при заказе наших услуг могут
            рассчитывать как крупные компании, так и частные лица.
          </p>
        </div>
        <div
          class="right justify-center w-[315px] h-[335px] lg:w-[700px] lg:h-[446px] lg:flex lg:justify-between lg:gap-5  bg-[#F8F8F8] rounded-3xl "
        >
          <div class="block-1 w-[143px] lg:w-[229px] h-[126px] lg:h-[197px] ml-[96px] pt-[20px] lg:pt-24   ">
            <div class="top flex justify-center">
              <p class="text-5xl lg:text-[88px] font-semibold lg:font-light w-[66px] lg:w-[106px] h-[71px] lg:h-[125px] ml-[10px] lg:ml-[-60px] pt-10 ">60</p>
              <p class="text-4xl font-medium w-6 h-14 text-brand mt-5 lg:mt-6">+</p>
            </div>
            <p class="text-lg lg:text-2xl font-normal text-[#67675F] pt-[30px]">Единиц техники</p>
          </div>
          <div class="block-2 w-[111px] lg:w-[232px] h-[111px] lg:h-[177px] mt-16 lg:pt-24  ml-auto mr-auto flex flex-col lg:gap-5 justify-center ">
            <p class="text-5xl lg:text-[88px] font-semibold lg:font-light  lg:mt-8 lg:h-full  text-center lg:pl-[0px] ">15</p>
            <p class="text-2xl  font-normal text-[#67675F] mt-4 text-center lg:pb-5">Карьеров</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
import TheTitle from "../../../ui/theTitle.vue";

export default {
  components: { TheTitle },
};
</script>
