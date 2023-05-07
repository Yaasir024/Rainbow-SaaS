<script setup>
const emits = defineEmits(["close"]);
</script>

<template>
  <div
    class="dropdown p-[32px] absolute top-[35px] left-[-20px] z-40 min-w-[320px]"
  >
    <ul class="">
      <li class="link mb-[26px]">
        <RouterLink to="/payment-service" @click="$emit('close')">
          <div class="flex items-center">
            <div class="ml-[16px]">
              <h2
                class=""
              >
                Payments
              </h2>
            </div>
          </div>
        </RouterLink>
      </li>
      <li class="link mb-[26px]">
        <RouterLink to="/business-incorporation" @click="$emit('close')">
          <div class="flex items-center">
            <div class="ml-[16px]">
              <h2
                class=""
              >
                Business Incorporation
              </h2>
            </div>
          </div>
        </RouterLink>
      </li>
      <li class="link">
        <RouterLink to="/" @click="$emit('close')">
          <div class="flex items-center">
            <div class="ml-[16px]">
              <h2
                class=""
              >
                Payroll and Tax
              </h2>
            </div>
          </div>
        </RouterLink>
      </li>
    </ul>
  </div>
</template>

<style scoped>
.dropdown {
  background: #ffffff;
  box-shadow: 0px 44px 116px rgba(0, 0, 0, 0.1);
  border-radius: 24px;
}
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
</style>
