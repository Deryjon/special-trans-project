<template>
<div class="for-example lg:flex lg:gap-10 mt-20 mb-10 lg:mt-10 lg:mb-10">
          <div class="img w-full lg:w-[580px] h-[222px] lg:h-[480px] rounded-lg">
            <img class="w-full h-full object-cover rounded-lg" :src="`${data.image}`" alt="" />
          </div>
          <div class="text mt-8 lg:mt-0 lg:w-[798px] lg:h-[406px]">
            <p class="title text-dark text-2xl font-medium lg:text-3xl lg:font-semibold">{{data.title}}</p>
            <p class="description text-[#67675F] hidden lg:block text-sm font-normal mt-5 lg:text-lg lg:text-dark">{{ data.descprition }}</p>
            <div class="price mt-6 lg:mt-14 ">
              <div class="price-1 flex items-center w-[324px] lg:w-[566px]">
                <p class="text-sm text-light text-dark ">Самосвал 20куб</p>
                <div class="bor h-0 w-[58px] lg:w-[310px] border-b pt-4 "></div>
                <p class=" text-light text-base">От <span class="text-brand text-base text-normal">{{ data.price1 }}</span> смена</p>
              </div>
              <div class="price-2 flex items-center w-[324px] mt-6 lg:w-[566px]">
                <p class="text-sm text-light text-dark ">Самосвал 25куб</p>
                <div class="bor h-0 w-[58px] lg:w-[310px] border-b pt-4 "></div>
                <p class=" text-light text-base">От <span class="text-brand text-base text-normal">{{ data.price2 }}</span> смена</p>
              </div>
              <div class="price-2 flex items-center w-[324px] mt-6 lg:w-[566px]">
                <p class="text-sm text-light text-dark ">Самосвал 30куб</p>
                <div class="bo h-0 w-[58px] lg:w-[310px] border-b pt-4 "></div>
                <p class=" text-light text-base">От <span class="text-brand text-base text-normal">{{ data.price3 }}</span> смена</p>
              </div>
            </div>
          </div>
        </div>

</template>
<script>
export default{
    props: {
        data: {
            type: Object,
            require: true
        }
    },
}
</script>