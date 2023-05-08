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
  setTimeout(() => {

    animate()
  }, '500')
})
</script>

<template>
  <section class="hero pt-[145px] overflow-hidden relative min-h-[calc(100vh_-_80px)]">
    <div class="flex flex-col items-center px-[20px] mb-[200px] xs:mb-[300px] md:mb-[350px] xl:mb-[420px]">
      <RouterLink to="/about" class="" id="badge-btn-1">
        <div class="badge-container px-[10px] py-[6px] flex items-center w-fit">
          <button
            class="text-[14px] leading-[20px] font-medium text-rb-dark tracking-[-0.01em] bg-[#EDEDF1] rounded-[20px] py-1 px-2 mr-[8px]">
            Rainbow 2023 Release</button><span
            class="text-[14px] leading-[20px] font-medium text-white tracking-[-0.01em] mr-[10px]">Join to waitlist</span>
          <img src="@/assets/icons/arrow-right.svg" alt="" class="" />
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
      class="absolute left-0 bottom-[0px] translate-y-[50%] xs:translate-y-[60%] block 2xl:hidden w-full" />
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
