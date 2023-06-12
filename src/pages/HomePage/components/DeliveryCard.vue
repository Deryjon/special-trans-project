<template>
  <div
    class="delivery-card w-[335px] lg:[653px] h-[44px] lg:h-[28px] flex  gap-5 lg:justify-between  mt-3 lg:mt-14"
  >
    <div class="icon w-[22px] h-[22px]   mt-3">
      <img class="w-full h-full" :src="`${data.image}`" alt="icon" />
    </div>
    
      <p class="text-base lg:text-xl   font-light text-[#1E1E1C] " >
        {{ data.name }}
      </p>
    
  </div>
</template>
<script>
export default {
  props: {
    data: {
      type: Object,
      require: true,
    },
  },
};
</script>
