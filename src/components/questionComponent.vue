<template>
  <section class="questions lg:bg-[#F8F8F8] mb-[70px]">
    <div class="container">
      <div class="wrapper lg:flex lg:justify-between w-full">
        <div class="left lg:w-[489px] lg:h-[362px] mt-10 lg:mt-24 lg:mb-[70px]">
          <TheTitle>Остались вопросы?</TheTitle>
          <p class="text-base lg:w-[280px] text-brand font-normal mt-6">
            Закажите обратный звонок и узнайте больше о наших услугах!
          </p>
          <p class="text-sm text-gray mt-2 w-[335px] lg:mt-5 lg:mb-12">
            Оставьте заявку и наш менеджер перезвонит вам в течении 10 минут
          </p>
          <TheButton class="hidden lg:block">Заказать звонок</TheButton>
        </div>
        <div
          class="back lg:bg-brand lg:w-[318px] lg:h-[588px] lg:absolute lg:right-[270px]"
        ></div>
        <div
          class="right lg:relative w-full   lg:w-[686px] h-[326px] lg:h-[475px] mt-8 lg:mt-14 text-sm p-4 lg:p-9 lg:mb-[57px]"
        >
          <input
            class="name w-full lg:w-[596px] h-[48px] lg:h-[65px] p-4 lg:p-8"
            type="text"
            placeholder="Имя"
          />
          <input
            class="number w-full lg:w-[596px] h-[48px] lg:h-[65px] p-4 lg:p-8 mt-4 text-sm"
            type="number"
            placeholder="Телефон"
          />
          <textarea
            name=""
            class="w-full lg:w-[593px] h-[128px] lg:h-[172px] p-4 lg:p-8 mt-4 text-sm text-left"
            placeholder="Комментарии"
            cols="78"
            rows="8"
          ></textarea>

          <p class="text-[16px ] font-normal text-[#181A28] mt-4">
            Соглашение о персональных данных
          </p>
        </div>
      </div>
    </div>
  </section>
</template>
<script>
import TheButton from "../ui/the-button.vue";
import TheTitle from "../ui/theTitle.vue";

export default {
  components: { TheTitle, TheButton },
};
</script>
<style lang="scss" scoped>
.wrapper {
  .right {
    background: #ffffff;
    box-shadow: 0px 4px 40px rgba(7, 17, 51, 0.07);
    border-radius: 12px;

    input,
    textarea {
      border: 1px #dddddd solid;
      border-radius: 6px;
      color: #181a28;
    }
    input::-webkit-outer-spin-button,
    input::-webkit-inner-spin-button {
      /* display: none; <- Crashes Chrome on hover */
      -webkit-appearance: none;
      margin: 0; /* <-- Apparently some margin are still there even though it's hidden */
    }
  }
}
</style>
