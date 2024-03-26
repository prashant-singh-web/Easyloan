<script lang="ts">
export default {}
</script>
<template>
  <div class="w-full flex flex-col p-5 md:p-20 bg-sky-100">
    <div class="w-full grid grid-cols-1 lg:grid-cols-3 gap-y-10 gap-5">
      <div class="w-full flex flex-col">
        <img src="../assets/logo2_footer.png.webp" alt="hiii" class="w-36" />
        <p class="texl-lg font-medium text-gray-800/70">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Nostrum eveniet ex reiciendis
          similique dolore quidem doloremque eligendi, labore quam temporibus.
        </p>
      </div>
      <div class="w-full grid grid-cols-2">
        <ul class="text-base space-y-2">
          <li class="font-bold text-lg">Quick Links</li>
          <li class="list-1">Work</li>
          <li class="list-1">Service</li>
          <li class="list-1">Products</li>
          <li class="list-1">Tips & Tricks</li>
        </ul>
        <ul class="text-base space-y-2">
          <li class="font-bold text-lg">Solution</li>
          <li class="list-1">Air freight</li>
          <li class="list-1">Ocean freight</li>
          <li class="list-1">Blog</li>
        </ul>
      </div>
      <div class="flex flex-col">
        <h2 class="text-xl font-bold text-gray-900">Newsletter</h2>
        <p class="my-3">Subscribe newsletter to get updates.</p>
        <div class="grid grid-cols-[70%_30%] border-[1.5px] border-sky-500 w-3/4">
          <input
            type="text"
            placeholder="Enter your email"
            class="outline-none p-2 text-sm w-full"
          />
          <div class="grid w-full bg-sky-500 place-items-center">
            <i class="fa-solid text-xl text-white fa-paper-plane"></i>
          </div>
        </div>
        <div class="flex flex-row mt-5 space-x-3">
          <i class="fa-brands socical-link fa-instagram"></i>
          <i class="fa-brands socical-link fa-facebook"></i>
          <i class="fa-brands socical-link fa-twitter"></i>
          <i class="fa-brands socical-link fa-youtube"></i>
        </div>
      </div>
    </div>
    <hr class="my-5" />
    <p class="mx-auto text-base">
      Copyright ©2024 All rights reserved | This template is made with Vuejs and Tailwind css by
      Prashant Singh
    </p>
  </div>
</template>
<style>
.list-1 {
  @apply hover:text-sky-500 hover:underline cursor-pointer w-fit ease-in-out duration-200;
}
.socical-link {
  @apply text-xl text-gray-950/90 cursor-pointer ease-linear duration-300 hover:text-sky-500;
}
</style>
