<script setup>
import BoltBtn from "@/components/buttons/TypeBolt.vue";
import BorderBtn from "@/components/buttons/TypeBorder.vue";
</script>

<template>
  <section class="bg-[#080841] pl-[110px]">
    <div class="pb-[80px]">
      <div class="w-[1.2px] h-[80px] mb-[24px] bg-white"></div>
      <h1
        class="text-[48px] leading-[57px] max-w-[490px] font-tomato text-white"
      >
        Discover how to achieve great revenue by
        <span class="text-rb-main">scaling to Africa</span>
      </h1>
      <div class="flex items-center mt-[52px]">
        <div class="mr-[16px]">
          <RouterLink to="/">
            <BoltBtn text="contact sales" />
          </RouterLink>
        </div>
        <div class="">
          <RouterLink to="/">
            <BorderBtn text="learn more" />
          </RouterLink>
        </div>
      </div>
    </div>
  </section>
</template>
