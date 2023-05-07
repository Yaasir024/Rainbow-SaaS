<script setup>
const props = defineProps(["text"]);
</script>

<template>
  <button
    class="bg-transparent btn text-white text-[16px] font-medium leading-[24px] capitalize px-[18px] py-[10px] rounded-lg border border-white hover:scale-105 transition-all duration-150 "
  >
    {{ text }}
  </button>
</template>
