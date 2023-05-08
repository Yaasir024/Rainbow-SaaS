<template>
  <section
    class="py-[165px] px-[28px] xs:px-[40px] md:px-[60px] lg:px-[95px] 2xl:px-[120px] flex items-center flex-col md:flex-row">
    <div class="md:flex-[50%]">
      <img src="@/assets/images/testimonial/img1.png" alt="" class="max-h-[380px] md:max-h-full" />
    </div>
    <div class="md:flex-[50%] md:ml-[40px] mt-[40px] md:mt-0" >
      <div class="flex items-center mb-[20px] md:mb-[30px]">
        <img src="@/assets/icons/Star.svg" alt="" class="mr-[8px]" v-for="i in 5" :key="i" />
      </div>
      <h2
        class="text-[20px] xs:text-[22px] md:text-[28px] lg:text-[36px] leading-[28px] xs:leading-[30px] md:leading-[36px] lg:leading-[42px] font-medium max-w-[580px] text-rb-primary-900 font-tomato">
        Rainbow made scaling into Africa effortless with their streamlined services, saving us time and resources. Highly
        recommend!
      </h2>
      <div class="mt-[32px] flex flex-col">
        <span class="text-[16px] leading-[24px] font-medium text-rb-primary-900 font-tomato">Benjamin Hughes</span>
        <span class="text-[14px] leading-[20px] tracking-[-0.01em] mt-[4px] text-rb-primary-900/60">CEO, Tellway
          Inc</span>
      </div>
      <div class="controls mt-[32px] flex items-center">
        <button class="h-[40px] w-[40px] rounded-full flex items-center justify-center mr-[16px] bg-rb-primary-900/5">
          <img src="@/assets/icons/arrow-left-line.svg" alt="" class="">
        </button>
        <button class="h-[40px] w-[40px] rounded-full flex items-center justify-center bg-rb-primary-900/5">
          <img src="@/assets/icons/arrow-right-line.svg" alt="" class="">
        </button>
      </div>
    </div>
  </section>
</template>
