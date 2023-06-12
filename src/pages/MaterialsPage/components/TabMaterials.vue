<template>
  <div class="tabs xl:w-[1400px] lg:1200px m-auto">
    <div class="nav-tabs flex " >
      <div
        class="nav-item text-xs text-[#1D1D1B99] border-b w-[325px] lg:w-[500px] h-8 border-[#1D1D1B99] lg:text-2xl lg:font-light flex justify-center items-center lg:cursor-pointer lg:duration-150 mt-8 "
        @click="setActive('tab-1')"
        :class="{ active: isActive('tab-1') }"
      >
        Песок
      </div>
      <div
        class="nav-item text-xs text-[#1D1D1B99] border-b w-[325px] lg:w-[500px] h-8 border-[#1D1D1B99] lg:text-2xl lg:font-light flex justify-center items-center lg:cursor-pointer lg:duration-150 mt-8"
        @click="setActive('tab-2')"
        :class="{ active: isActive('tab-2') }"
      >
        Щебень
      </div>
      <div
        class="nav-item text-xs  text-[#1D1D1B99] border-b w-[500px] lg:w-[500px] h-8 border-[#1D1D1B99] lg:text-2xl lg:font-light flex justify-center items-center lg:cursor-pointer lg:duration-150 mt-8"
        @click="setActive('tab-3')"
        :class="{ active: isActive('tab-3') }"
      >
        Асфальтовая крошка
      </div>
    </div>
    <div class="tab-content lg:mt-24 mt-8">
      <div class="tab-panel" v-show="isActive('tab-1')">
        <div class="for-example lg:flex lg:gap-10">
          <div class="img w-full lg:w-[580px] h-[222px] lg:h-[480px] rounded-lg">
            <img class="w-full h-full rounded-lg" src="../../../assets/images/material-1.jpg" alt="" />
          </div>
          <div class="text mt-8 lg:mt-0 lg:w-[798px] lg:h-[406px]">
            <p class="title text-dark text-2xl font-medium lg:text-3xl lg:font-semibold">Песок</p>
            <p class="description text-[#67675F] text-sm font-normal mt-5 lg:text-lg lg:text-dark">Материал мелкого размера применяют для производства сухих смесей. Песок с частицами средней величины используют при изготовлении бетонов для всех типов растворов. Крупные фракции используют для создания покрытий, оснований и несущих конструкций, испытывающих мощные нагрузки</p>
            <div class="price mt-6 lg:mt-14">
              <div class="price-1 flex items-center w-[324px] lg:w-[566px]">
                <p class="text-sm  text-light text-dark ">Песок карьерный 1.91</p>
                <div class="bor h-0 w-[106px] lg:w-[328px] border-b pt-4 "></div>
                <p class=" text-light text-base">От <span class="text-brand text-base text-normal"> 160 ₽</span></p>
              </div>
              <div class="price-2 flex items-center w-[323px] lg:w-[566px] mt-6">
                <p class="text-sm text-light text-dark ">Песок карьерный 1.40</p>
                <div class="bor h-0 w-[102px] lg:w-[323px] border-b pt-4 "></div>
                <p class=" text-light text-base">От <span class="text-brand text-base text-normal"> 160 ₽</span></p>
              </div>
              <div class="price-2 flex items-center w-[324px] lg:w-[566px] mt-6">
                <p class="text-sm text-light text-dark ">Песок карьерный 1.10</p>
                <div class="bor h-0 w-[105px] lg:w-[327px] border-b pt-4 "></div>
                <p class=" text-light text-base">От <span class="text-brand text-base text-normal"> 160 ₽</span></p>
              </div>
              <div class="price-2 flex items-center w-[324px] lg:w-[566px] mt-6">
                <p class="text-sm text-light text-dark ">Песок намывной</p>
                <div class="bor h-0 w-[136px] lg:w-[362px] border-b pt-4 "></div>
                <p class=" text-light text-base">От <span class="text-brand text-base text-normal"> 250 ₽</span></p>
              </div>
              
            </div>
          </div>
        </div>
      </div>
      <!-- !!! -->
      <div class="tab-panel mt-8" v-show="isActive('tab-2')" >
        <div class="for-example lg:flex lg:gap-10">
          <div class="img w-full lg:w-[580px] h-[222px] lg:h-[480px] rounded-lg">
            <img class="w-full h-full object-cover rounded-lg" src="../../../assets/images/material-2.jpg" alt="" />
          </div>
          <div class="text mt-8 lg:mt-0 lg:w-[798px] lg:h-[406px]">
            <p class="title text-dark text-2xl font-medium lg:text-3xl lg:font-semibold">Щебень</p>
            <p class="description text-[#67675F] text-sm font-normal mt-5 lg:text-lg lg:text-dark">Щебень размером 5-20 мм. Это самый востребованный в строительстве и <span class="text-brand text-base text-normal underline">производстве ЖБИ</span> материал, его также применяют для строительства дорог и создания фундамента. Такой щебень незаменим и в частном строительстве при подготовке бетона. Щебень 20-40 мм. Используется в дренажных работах, при строительстве трамвайных и железнодорожных путей, а также может применяться при обустройстве фундаментов зданий промышленного назначения. Щебень размером 40-70 мм может использовать для дренажа, добавляться в бетон и бетонные изделия;</p>
            <div class="price mt-6 lg:mt-14">
              <div class="price-1 flex items-center w-[324px] lg:w-[566px]">
                <p class="text-sm text-light text-dark ">Щебень гранитный фр. 5-20 </p>
                <div class="bor h-0 w-[60px] lg:w-[277px] border-b pt-4 "></div>
                <p class=" text-light text-base">От <span class="text-brand text-base text-normal"> 800 ₽</span></p>
              </div>
              <div class="price-2 flex items-center w-[324px] mt-6 lg:w-[566px]">
                <p class="text-sm text-light text-dark ">Щебень гранитный фр. 20-40</p>
                <div class="bor h-0 w-[51px] lg:w-[266px] border-b pt-4 "></div>
                <p class=" text-light text-base">От <span class="text-brand text-base text-normal"> 600 ₽</span></p>
              </div>
              <div class="price-2 flex items-center w-[324px] mt-6 lg:w-[566px]">
                <p class="text-sm text-light text-dark ">Щебень гравийный фр. 5-20</p>
                <div class="bor h-0 w-[60px] lg:w-[276px] border-b pt-4 "></div>
                <p class=" text-light text-base">От <span class="text-brand text-base text-normal"> 500 ₽</span></p>
              </div>
              <div class="price-2 flex items-center w-[324px] mt-6 lg:w-[566px]">
                <p class="text-sm text-light text-dark ">Гранитный отсев</p>
                <div class="bor h-0 w-[132px] lg:w-[345px] border-b pt-4 "></div>
                <p class=" text-light text-base">От <span class="text-brand text-base text-normal"> 1000 ₽</span></p>
              </div>
              
            </div>
          </div>
        </div>
      </div>
      <!-- !!! -->
      <div class="tab-panel mt-8" v-show="isActive('tab-3')">
        <div class="for-example lg:flex lg:gap-10">
          <div class="img w-full lg:w-[580px] h-[222px] lg:h-[480px] rounded-lg">
            <img class="w-full h-full object-cover rounded-lg" src="../../../assets/images/material-4.jpg" alt="" />
          </div>
          <div class="text mt-8 lg:mt-0 lg:w-[798px] lg:h-[406px]">
            <p class="title text-dark text-2xl font-medium lg:text-3xl lg:font-semibold">Вторичные материалы</p>
            <div class="price mt-6 lg:mt-14 ">
              <div class="price-1 flex items-center w-[324px] lg:w-[566px]">
                <p class="text-sm text-light text-dark ">Асфальтная крошка</p>
                <div class="bor h-0 w-[115px] lg:w-[335px] border-b pt-4 "></div>
                <p class=" text-light text-base">От <span class="text-brand text-base text-normal"> 500 ₽</span></p>
              </div>
              <div class="price-2 flex items-center w-[324px] mt-6 lg:w-[566px]">
                <p class="text-sm text-light text-dark ">Бой кирпича</p>
                <div class="bor h-0 w-[162px] lg:w-[383px] border-b pt-4 "></div>
                <p class=" text-light text-base">От <span class="text-brand text-base text-normal"> 200 ₽</span></p>
              </div>
              <div class="price-2 flex items-center w-[324px] mt-6 lg:w-[566px]">
                <p class="text-sm text-light text-dark ">Бой бетона</p>
                <div class="bor h-0 w-[171px] lg:w-[393px] border-b pt-4 "></div>
                <p class=" text-light text-base">От <span class="text-brand text-base text-normal"> 200 ₽</span></p>
              </div>

              
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data: () => ({
    activeTab: "tab-1",
  }),
  methods: {
    setActive(tab) {
      this.activeTab = tab;
    },
    isActive(tab) {
      return this.activeTab === tab;
    },
  },
};

</script>
<style lang="scss" scoped>
.tabs {
 
  & .active {
    @apply text-brand border-b-brand font-normal border-b-2;
  }
}
</style>
