<script setup>
import BoltBtn from "@/components/buttons/TypeBolt.vue";
import BorderBtn from "@/components/buttons/TypeBorder.vue";
</script>

<template>
  <section class="hero pt-[145px] overflow-hidden">
    <div class="flex flex-col items-center px-[20px] mb-[60px]">
      <RouterLink to="/about" class=""
        ><div
          class="badge-container px-[10px] py-[6px] flex items-center w-fit"
        >
          <button
            class="text-[14px] leading-[20px] font-medium text-rb-dark tracking-[-0.01em] bg-[#EDEDF1] rounded-[20px] py-1 px-2 mr-[8px]"
          >
            Rainbow 2023 Release</button
          ><span
            class="text-[14px] leading-[20px] font-medium text-white tracking-[-0.01em] mr-[10px]"
            >Join to waitlist</span
          >
          <img src="@/assets/icons/arrow-right.svg" alt="" class="" /></div
      ></RouterLink>

      <h1
        class="text-[30px] sm:text-[48px] md:text-[64px] leading-[38px] sm:leading-[54px] md:leading-[68px] tracking-[-0.02em] font-semibold max-w-[835px] mt-[38px] font-tomato text-white text-center"
      >
        <span class="text-rb-main">Rainbow</span> is revolutionizing Global
        Commerce.
      </h1>
      <p
        class="text-[16px] sm:text-[20px] leading-[20px] sm:leading-[28px] tracking-[-0.014em] max-w-[580px] mt-[24px] text-white text-center"
      >
        Enabling global businesses to scale in Africa without paperwork
      </p>
      <div class="flex items-center mt-[32px]">
        <div class="mr-[16px]">
          <RouterLink to="/">
            <BoltBtn text="get started" />
          </RouterLink>
        </div>
        <div class="">
          <RouterLink to="/">
            <BorderBtn text="learn more" />
          </RouterLink>
        </div>
      </div>
    </div>
    <!-- <img
      src="@/assets/images/home/map.svg"
      alt=""
      class="mb-[-500px] xs:mb-[-450px] sm:mb-[-370px]"
    /> -->
  </section>
</template>

<style scoped>
.hero {
  background-image: url(./../../../images/bg/hero-bg-min.png);
  background-repeat: no-repeat;
  background-size: cover;
}
.badge-container {
  background: rgba(255, 255, 255, 0.1);

  border: 1px solid #dcdae2;
  border-radius: 20px;
}
</style>
