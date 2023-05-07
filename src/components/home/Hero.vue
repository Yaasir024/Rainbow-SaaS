<template>
  <section class="hero flex flex-col items-center px-[20px] pt-[145px] min-h-screen bg-blue-500">
    <RouterLink to="/about" class=""
      ><div class="badge-container px-[10px] py-[6px] flex items-center w-fit">
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
      class="text-[30px] sm:text-[48px] md:text-[64px] leading-[38px] sm:leading-[54px] md:leading-[68px] font-semibold max-w-[835px] mt-[38px] font-tomato text-white text-center"
    >
      <span class="text-rb-main">Rainbow</span> is revolutionizing Global
      Commerce.
    </h1>
    <p
      class="text-[16px] sm:text-[20px] leading-[20px] sm:leading-[28px] max-w-[580px] mt-[24px] text-white text-center"
    >
      Enabling global businesses to scale in Africa without paperwork
    </p>
    <!-- <img src="@/assets/images/home/hero-illustration.svg" alt="" class="" /> -->
  </section>
</template>

<style scoped>
.badge-container {
  background: rgba(255, 255, 255, 0.1);

  border: 1px solid #dcdae2;
  border-radius: 20px;
}
</style>
