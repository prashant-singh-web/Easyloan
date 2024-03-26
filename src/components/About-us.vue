<script lang="ts">
export default {}
</script>
<template>
  <div
    class="w-full bg-sky-200 pb-10 md:p-10 md:py-20 grid grid-cols-1 md:grid-cols-2 place-items-center"
  >
    <div class="w-fit relative">
      <img
        src="../assets/about1.jpg.webp"
        alt="img"
        class="w-full aspect-square md:w-[80%] sm:p-1 md:aspect-square rounded-md mx-auto"
      />
      <div
        class="absolute size-[14rem] hidden lg:flex rounded-md bg-sky-500 -right-6 -bottom-10 flex-col items-center justify-center"
      >
        <h4 class="text-6xl font-black text-white">99%</h4>
        <p class="text-white">Customer Satisfaction</p>
      </div>
    </div>
    <div class="flex md:ml-auto flex-col w-[80%]">
      <h3 class="text-xl my-2 md:my-0 md:text-3xl lg:text-4xl font-bold text-sky-800">
        We guide projects and organizations in making the right decisions.
      </h3>
      <p class="text-sm md:text-base text-gray-800/60 my-5 font-medium">
        Tools such as a profit simulator and tax calculator show the value of your stock options and
        exercise cost. The brochure must grab a viewer’s attention and hold it long enough to
        deliver the pertinent information.
      </p>
      <div class="w-full p-[0.5px] bg-gray-500 my-5"></div>

      <ul
        class="list-disc list-inside text-sky-600 text-sm md:text-lg font-semibold space-y-3 mt-5"
      >
        <li><span class="text-gray-950/70">Monthly recurring revenue</span></li>
        <li><span class="text-gray-950/70">Customer acquisition cost</span></li>
        <li><span class="text-gray-950/70">Number of customers</span></li>
      </ul>
      <button class="button-sky">Learn More</button>
    </div>
  </div>
</template>
<style>
.button-sky {
  @apply w-fit px-7 py-2 text-base border-2 border-sky-500 text-sky-500 mt-5 hover:bg-sky-500 hover:text-white ease-in-out duration-300;
}
.List-text {
  @apply text-gray-950/70;
}
</style>
