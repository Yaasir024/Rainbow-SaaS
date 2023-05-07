<script setup>
import BoltBtn from "@/components/buttons/TypeBolt.vue";
import FullBtn from "@/components/buttons/TypeFull.vue";
</script>

<template>
  <section class="hero flex flex-col 2xl:flex-row justify-between bg-[#45DEFE]/20 pt-[80px] ">
    <div class="flex flex-col items-center md:items-start pl-[40px] md:pl-[110px] pr-[40px] xl:pr-0 pt-[65px] pb-[156px]">
      <RouterLink to="/" class=""
        ><div
          class="badge-container px-[10px] py-[6px] flex items-center w-fit"
        >
          <button
            class="text-[14px] leading-[20px] font-medium text-rb-dark tracking-[-0.01em] bg-[#EDEDF1] rounded-[20px] py-1 px-2 mr-[8px]"
          >
            Global Payment Service
          </button>
          <img
            src="@/assets/icons/arrow-right-black.svg"
            alt=""
            class=""
          /></div
      ></RouterLink>
      <h1
        class="text-[30px] sm:text-[48px] md:text-[64px] leading-[38px] sm:leading-[54px] md:leading-[68px] font-semibold max-w-[580px] mt-[32px] font-tomato text-rb-dark text-center md:text-left"
      >
        Get Access to Payment Services, Increase Revenue
      </h1>
      <p
        class="mt-[24px] text-[20px] leading-[28px] max-w-[580px] tracking-[-0.014em] text-rb-primary-900/60  text-center md:text-left"
      >
        Connect with your customers and increase sales in Africa with our
        reliable payment collection infrastructure
      </p>
      <div class="flex items-center flex-col xs:flex-row mt-[32px]">
        <div class="mb-[20px] xs:mb-0 xs:mr-[16px]">
          <RouterLink to="/">
            <BoltBtn text="get started" />
          </RouterLink>
        </div>
        <div class="">
          <RouterLink to="/">
            <FullBtn text="try rainbow free" />
          </RouterLink>
        </div>
      </div>
    </div>
    <img src="@/assets/images/home/cta.png" alt="" class="hidden 2xl:block h-[650px]">
  </section>
</template>

<style scoped>
.badge-container {
  background: white;

  border: 1px solid #dcdae2;
  border-radius: 20px;
}
</style>
