<template>
  <div class="header-actions ml-auto">
    <TheButton class="hidden lg:block" >
      Заказать вызов
    </TheButton>
    <button class="burger-btn w-5 h-5 flex justify-center items-center lg:hidden" @click="$emit('openMenu')">
      <img src="@/assets/icons/burger.svg" alt="burger-btn">

    </button>
  </div>
</template>
<script>
import TheButton from '../../../ui/the-button.vue';

export default {
    components: { TheButton }
};
</script>
