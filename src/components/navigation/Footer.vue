<template>
  <footer class="">
    <div class="bg-white pt-[48px] px-[40px] md:px-[120px] pb-[165px] flex flex-col md:flex-row md:justify-between">
      <img src="@/assets/logo/icon.svg" alt="" class="h-[42px] w-[42px]" />
      <div class="flex flex-col xs:flex-row mt-[20px] md:mt-0">
        <ul class="mr-[36px] mb-[20px]">
          <li class="alpha-black mb-[8px]">Products</li>
          <li class="link mb-[8px]">
            <RouterLink to="/payment-service"> Payments </RouterLink>
          </li>
          <li class="link mb-[8px]">
            <RouterLink to="/business-incorporation"> Business Incorporation </RouterLink>
          </li>
          <li class="link">
            <RouterLink to="/"> Payroll and Tax </RouterLink>
          </li>
        </ul>
        <ul class="mr-[36px] mb-[20px]">
          <li class="alpha-black mb-[8px]">Company</li>
          <li class="link mb-[8px]">
            <RouterLink to="/"> About us </RouterLink>
          </li>
          <li class="link mb-[8px]">
            <RouterLink to="/"> Contact </RouterLink>
          </li>
          <li class="link">
            <RouterLink to="/"> FAQ </RouterLink>
          </li>
        </ul>
        <ul class=" mb-[20px]">
          <li class="alpha-black mb-[8px]">Legal</li>
          <li class="link mb-[8px]">
            <RouterLink to="/"> Terms of use </RouterLink>
          </li>
          <li class="link">
            <RouterLink to="/"> Privacy </RouterLink>
          </li>
        </ul>
      </div>
    </div>
    <div class="px-[40px] md:px-[120px] py-[24px] bg-[#EFFAF9] flex items-center justify-between flex-col xs:flex-row">
        <span class="rights text-base">Rainbow. All right reserved. © 2023</span>
        <div class="socials flex items-center mt-[20px] xs:mt-0">
            <img src="@/assets/icons/social/facebook.svg" alt="" class="mr-[16px]">
            <img src="@/assets/icons/social/twitter.svg" alt="" class="mr-[16px]">
            <img src="@/assets/icons/social/github.svg" alt="" class="">
        </div>
    </div>
  </footer>
</template>

<style scoped>
.alpha-black {
  font-size: 16px;
  line-height: 24px;
  font-weight: 500;
  color: rgba(47, 43, 67, 0.6);
}
.link {
  font-size: 16px;
  line-height: 24px;
  font-weight: 500;
}
.rights {
    color: rgba(47, 43, 67, 0.6);
}
</style>
