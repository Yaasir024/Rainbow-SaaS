<script setup>
const props = defineProps(["text"]);
</script>

<template>
  <button
    class="bg-rb-main btn text-rb-dark text-[16px] font-medium leading-[24px] capitalize px-[18px] py-[10px] rounded-lg hover:scale-105 transition-all duration-150 ease-in-out flex items-center">
    <svg width="10" height="18" viewBox="0 0 10 18" fill="none" xmlns="http://www.w3.org/2000/svg" class="mr-[14px]">
      <path d="M6.25 1.5L1.25 9H8.75L3.75 16.5" stroke="#000034" stroke-width="1.5" stroke-linecap="round"
        stroke-linejoin="round" />
    </svg>
    {{ text }}
  </button>
</template>
