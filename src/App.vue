<script setup lang="ts">
import { RouterView } from 'vue-router'
import HeaderNav from './components/Header-nav.vue'
import FooterSection from './components/Footer-Section.vue'
</script>

<template>
  <div class="w-full flex flex-col">
    <HeaderNav />

    <RouterView />
    <FooterSection />
  </div>
</template>

<style scoped></style>
