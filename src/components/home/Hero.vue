<script setup>
import { onMounted } from "vue";
import gsap from "gsap";
import BoltBtn from "@/components/buttons/TypeBolt.vue";
import BorderBtn from "@/components/buttons/TypeBorder.vue";

let tl = gsap.timeline({ yoyo: true, defaults: { opacity: 0, ease: "back" } });

const animate = () => {
  tl.from("#hero-main-text", { y: -80, duration: .6 })
    .from("#hero-excerpt", { y: -40, duration: .6 }, "-=0.2")
    .from("#hero-buttons", { y: -25, duration: .6 }, "-=0.2")
    .from("#badge-btn-1", { y: 50, duration: .6 }, "-=0.6")
}

onMounted(() => {
  animate()
  setTimeout(() => {

  }, '500')
})
</script>

<template>
  <section class="hero pt-[145px] overflow-hidden relative 2xl:min-h-[calc(100vh_-_80px)]">
    <div class="flex flex-col items-center px-[20px] mb-[200px] xs:mb-[300px] md:mb-[350px] xl:mb-[420px]">
      <RouterLink to="/about" class="" id="badge-btn-1">
        <div class="badge-container px-[10px] py-[6px] flex items-center w-fit">
          <button
            class="text-[14px] leading-[20px] font-medium text-rb-dark tracking-[-0.01em] bg-[#EDEDF1] rounded-[20px] py-1 px-2 mr-[8px]">
            Rainbow 2023 Release</button><span
            class="text-[14px] leading-[20px] font-medium text-white tracking-[-0.01em] mr-[10px]">Join to waitlist</span>
          <svg width="11" height="12" viewBox="0 0 11 12" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path
              d="M8.28134 5.33312L4.70534 1.75712L5.64801 0.814453L10.8333 5.99979L5.64801 11.1851L4.70534 10.2425L8.28134 6.66645H0.166672V5.33312H8.28134Z"
              fill="white" />
          </svg>
        </div>
      </RouterLink>

      <h1
        class="text-[30px] sm:text-[48px] md:text-[64px] leading-[38px] sm:leading-[54px] md:leading-[68px] tracking-[-0.02em] font-semibold max-w-[835px] mt-[38px] font-tomato text-white text-center"
        id="hero-main-text">
        <span class="text-rb-main">Rainbow</span> is revolutionizing Global
        Commerce.
      </h1>
      <p class="text-[16px] sm:text-[20px] leading-[20px] sm:leading-[28px] tracking-[-0.014em] max-w-[580px] mt-[24px] text-white text-center"
        id="hero-excerpt">

        Enabling global businesses to scale in Africa without paperwork
      </p>
      <div class="flex items-center mt-[32px]" id="hero-buttons">
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
    <img src="@/assets/images/home/map.svg" alt=""
      class="absolute left-0 bottom-[0px] translate-y-[50%] xs:translate-y-[60%] block w-full" />
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
