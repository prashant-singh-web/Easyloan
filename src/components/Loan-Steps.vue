<script lang="ts">
export default {}
</script>
<template>
  <main class="w-full bg-sky-200 p-10 py-20 grid grid-cols-1 md:grid-cols-2 place-items-center">
    <div class="flex md:ml-auto flex-col w-[80%]">
      <h3 class="text-4xl font-bold text-sky-800">Get loan in 3 easy steps</h3>
      <p class="text-base text-gray-800/60 my-5 font-medium">
        Tools such as a profit simulator and tax calculator show the value of your stock options and
        exercise cost. The brochure must grab a viewer’s attention and hold it long enough to
        deliver the pertinent information.
      </p>
      <div class="w-full p-[0.5px] bg-gray-500 my-5"></div>
      <ul class="list-disc list-inside text-sky-600 text-lg font-semibold space-y-3 mt-5">
        <li><span class="text-gray-950/70">Monthly recurring revenue</span></li>
        <li><span class="text-gray-950/70">Customer acquisition cost</span></li>
        <li><span class="text-gray-950/70">Number of customers</span></li>
      </ul>
      <button class="button-sky">Learn More</button>
    </div>
    <div class="w-fit hidden md:block">
      <img
        src="../assets/about1.jpg.webp"
        alt="img"
        class="w-3/4 aspect-square rounded-md mx-auto"
      />
    </div>
  </main>
</template>
<style>
.button-sky {
  @apply w-fit px-7 py-2 text-base border-2 border-sky-500 text-sky-500 mt-5 hover:bg-sky-500 hover:text-white ease-in-out duration-300;
}
.List-text {
  @apply text-gray-950/70;
}
</style>
