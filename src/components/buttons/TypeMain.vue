<script setup>
const props = defineProps(["text"]);
</script>

<template>
  <button
    class="bg-rb-main btn text-rb-dark text-[16px] font-medium leading-[24px] capitalize px-[18px] py-[10px] rounded-lg hover:scale-105 transition-all duration-150 ease-in-out"
  >
    {{ text }}
  </button>
</template>
