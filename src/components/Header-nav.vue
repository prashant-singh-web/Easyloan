<template>
  <div
    class="w-full flex flex-row justify-between fixed z-50 backdrop-blur-md bg-sky-500/50 p-3"
  >
    <img src="../assets/logo.png.webp" alt="hiii" class="w-28" />
    <div :class="menuOpen ? 'hide' : 'show'">
      <RouterLink to="/">Home</RouterLink>
      <RouterLink to="/about">About</RouterLink>
      <RouterLink to="/services">Services</RouterLink>
      <RouterLink to="/contact">Contact Us</RouterLink>
      <RouterLink to="/apply" class="bg-sky-700 shadow rounded-md px-5 py-2"
        >Apply for Loan</RouterLink
      >
    </div>

    <!-- Toggle button -->
    <button @click="toggleMenu" class="md:hidden text-white">
      <i class="fa-solid text-xl" :class="menuOpen ? 'fa-times' : 'fa-bars'"></i>
    </button>
  </div>
</template>

<script setup lang="ts">
import { ref } from "vue";
import { RouterLink } from "vue-router";

const menuOpen = ref(false);

const toggleMenu = () => {
  menuOpen.value = !menuOpen.value;
  console.log(menuOpen);
};
</script>

<style scoped>
.show {
  @apply hidden md:flex flex-row justify-center text-sm font-bold text-white items-center space-x-10;
}
.hide {
  @apply absolute md:static top-14 left-0 w-full md:w-fit bg-sky-600 md:bg-transparent flex flex-col md:flex-row justify-center text-sm font-bold text-white py-10 md:py-0 space-y-5 md:space-x-10 md:space-y-0  items-center;
}
</style>
