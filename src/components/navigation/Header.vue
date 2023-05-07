<script setup>
import { ref, onMounted } from "vue";

import { useClickOutside } from "@/composables/useClickOutside";

import MainBtn from "@/components/buttons/TypeMain.vue";

const showProductsMenu = ref(false);
const productMenu = ref(null);

useClickOutside(productMenu, () => {
  showProductsMenu.value = false;
});
</script>

<template>
  <header
    class="fixed top-0 left-0 right-0 bg-white flex items-center justify-between h-[80px] px-[20px] sm:px-[45px] md:px-[75px] xl:px-[112px] z-20"
  >
    <div class="flex items-center">
      <RouterLink to="/">
        <img src="@/assets/logo/main.svg" alt="" class="" />
      </RouterLink>
      <nav class="hidden lg:block ml-[45px]">
        <ul class="flex items-center">
          <li class="link mr-[32px] relative" ref="productMenu">
            <div
              class="flex items-center cursor-pointer"
              @click="showProductsMenu = !showProductsMenu"
            >
              <span class="mr-[13px]">Products</span>
              <button class="chevron">
                <svg
                  width="13"
                  height="8"
                  viewBox="0 0 13 8"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M1.26196 1.5L6.26196 6.5L11.262 1.5"
                    stroke="currentColor"
                    stroke-width="1.67"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                </svg>
              </button>
            </div>
            <!-- <transition name="menu">
              <FeaturesMenu
                v-if="showFeaturesMenu"
                @close="showFeaturesMenu = false"
              />
            </transition> -->
          </li>
          <li class="link mr-[32px]">
            <RouterLink to="/">
              <span class="text-base font-medium text-rb-gray-500"
                >About us</span
              >
            </RouterLink>
          </li>
          <li class="link">
            <RouterLink to="/">
              <span class="text-base font-medium text-rb-gray-500"
                >Contact</span
              >
            </RouterLink>
          </li>
        </ul>
      </nav>
    </div>
    <div class="flex items-center">
      <div class="mr-[30px]">
        <RouterLink to="/">
          <button class="text-rb-gray-500">Log in</button>
        </RouterLink>
      </div>
      <div class="hidden lg:block">
        <RouterLink to="/">
          <MainBtn text="register" />
        </RouterLink>
      </div>
      <div class="block lg:hidden">
        <button class="flex items-center justify-center">
          <svg
            width="32"
            height="32"
            viewBox="0 0 32 32"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <rect x="6" y="11.5" width="20" height="1.5" fill="#FAFAFA"></rect>
            <path
              d="M7 12.5H25"
              stroke="#1C1D1F"
              stroke-width="2.5"
              stroke-linecap="round"
            ></path>
            <path
              d="M7 19.5H25"
              stroke="#1C1D1F"
              stroke-width="2.5"
              stroke-linecap="round"
            ></path>
          </svg>
        </button>
      </div>
    </div>
  </header>
</template>

<style scoped>
.link span {
  font-weight: 500;
  font-size: 16px;
  line-height: 24px;

  color: #667085;
  transition: all 0.3s ease;
}

.link:hover span {
  color: #45defe;
}
.link .chevron {
  color: #667085;

  transition: all 0.3s ease;
}
.link:hover .chevron {
  /* color: #ff3a31;
  transform: rotate(180deg); */
  color: #45defe;
}

/* Nav Animation */
.nav-enter-active,
.nav-leave-active {
  transition: all 0.4s ease;
}
.nav-enter-from,
.nav-leave-to {
  opacity: 0;
  transform: translateX(100%);
}

/* Menu Animation */
.menu-enter-active,
.menu-leave-active {
  transition: transform 0.3s ease;
  transform-origin: top left;
}

.menu-enter-from,
.menu-leave-to {
  transform: scale(0);
}
</style>
