<script setup lang="ts"></script>

<template>
  <div class="w-full flex flex-row justify-between fixed z-50 backdrop-blur-md bg-sky-500/50 p-3">
    <img src="../assets/logo.png.webp" alt="hiii" class="w-28" />
    <div
      class="hidden md:flex flex-row justify-center text-sm font-bold text-white items-center space-x-16"
    >
      <RouterLink to="/">Home</RouterLink>
      <RouterLink to="/about">About</RouterLink>
      <RouterLink to="/services">Serviecs</RouterLink>
      <RouterLink to="/contact">Contact Us</RouterLink>
      <RouterLink to="/apply" class="bg-sky-700 shadow rounded-md px-5 py-2"
        >Apply for Loan</RouterLink
      >
    </div>
  </div>
</template>

<style scoped></style>
