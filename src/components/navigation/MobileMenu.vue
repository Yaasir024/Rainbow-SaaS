<script setup>
const emits = defineEmits(["close"]);
</script>



<template>
  <div
    class="font-sharp fixed top-0 left-0 h-screen w-screen bg-white text-black z-50"
  >
    <div class="flex items-center justify-between py-6 px-12 border-b">
      <RouterLink to="/">
        <img src="@/assets/logo/main.svg" alt="" class="" />
      </RouterLink>

      <button class="flex items-center justify-center"  @click="$emit('close')">
        <svg width="24" height="24" clip-rule="evenodd" fill-rule="evenodd" stroke-linejoin="round" stroke-miterlimit="2" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path d="m12 10.93 5.719-5.72c.146-.146.339-.219.531-.219.404 0 .75.324.75.749 0 .193-.073.385-.219.532l-5.72 5.719 5.719 5.719c.147.147.22.339.22.531 0 .427-.349.75-.75.75-.192 0-.385-.073-.531-.219l-5.719-5.719-5.719 5.719c-.146.146-.339.219-.531.219-.401 0-.75-.323-.75-.75 0-.192.073-.384.22-.531l5.719-5.719-5.72-5.719c-.146-.147-.219-.339-.219-.532 0-.425.346-.749.75-.749.192 0 .385.073.531.219z"/></svg>
      </button>
    </div>
    <div class="h-full flex items-center justify-center">
        <ul class="flex flex-col items-center mt-[-100px]">
          <li class="link ">
            <RouterLink to="/"  @click="$emit('close')">
              <span class="text-base font-medium text-rb-gray-500"
                >Home</span
              >
            </RouterLink>
          </li>
          <li class="link ">
            <RouterLink to="/payment-service"  @click="$emit('close')">
              <span class="text-base font-medium text-rb-gray-500"
                >Payments</span
              >
            </RouterLink>
          </li>
          <li class="link ">
            <RouterLink to="/business-incorporation"  @click="$emit('close')">
              <span class="text-base font-medium text-rb-gray-500"
                >Business Incorporation</span
              >
            </RouterLink>
          </li>
          <li class="link ">
            <RouterLink to="/about"  @click="$emit('close')">
              <span class="text-base font-medium text-rb-gray-500"
                >About us</span
              >
            </RouterLink>
          </li>
          <li class="link">
            <RouterLink to="/"  @click="$emit('close')">
              <span class="text-base font-medium text-rb-gray-500"
                >Contact</span
              >
            </RouterLink>
          </li>
        </ul>
    </div>
  </div>
</template>

<style scoped>
.link {
    margin-bottom: 8px;
}
.link span {
  font-weight: 500;
  font-size: 18px;
  line-height: 24px;

  color: #667085;
  transition: all 0.3s ease;
}

.link:hover span {
  color: #45defe;
}
</style>
