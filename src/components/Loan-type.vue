<template>
  <div id="service" class="w-full flex flex-col py-20 px-10 text-black justify-center items-center">
    <h2 class="text-2xl font-extrabold md:text-4xl text-center">
      Solutions for every business need.
    </h2>
    <hr class="w-16 h-1 bg-sky-500 mx-auto my-5" />
    <p class="text-xs md:text-sm font-semibold text-gray-800 text-center">
      The brochure must grab a viewer’s attention and hold it long <br />
      enough to deliver the pertinent information.
    </p>
    <div class="w-full grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-5 mt-10">
      <div class="w-full flex flex-col group">
        <i class="fa icon-style fa-home" aria-hidden="true"></i>
        <h3 class="loan-label">Home Loan</h3>
        <h5 class="loan-heading">What are my options and the cost to exercise?</h5>
        <p class="loan-paragraph">
          Tools such as a profit and tax calculator show the value of your stock options and
          exercise cost.
        </p>
      </div>
      <div class="w-full flex flex-col group">
        <i class="fa icon-style fa-car" aria-hidden="true"></i>
        <h3 class="loan-label">Car Loan</h3>
        <h5 class="loan-heading">What are my options and the cost to exercise?</h5>
        <p class="loan-paragraph">
          Tools such as a profit and tax calculator show the value of your stock options and
          exercise cost.
        </p>
      </div>
      <div class="w-full flex flex-col group">
        <i class="fa-solid icon-style fa-business-time" aria-hidden="true"></i>
        <h3 class="loan-label">Business Loan</h3>
        <h5 class="loan-heading">What are my options and the cost to exercise?</h5>
        <p class="loan-paragraph">
          Tools such as a profit and tax calculator show the value of your stock options and
          exercise cost.
        </p>
      </div>
    </div>
  </div>
</template>
<script lang="ts">
export default {}
</script>

<style>
.icon-style {
  @apply text-2xl md:text-5xl text-sky-400;
}
.loan-label {
  @apply text-base my-2 md:my-5 text-sky-500;
}
.loan-heading {
  @apply text-xl md:text-3xl font-bold group-hover:text-sky-500;
}
.loan-paragraph {
  @apply text-sm md:text-lg font-medium text-gray-950/70 my-3 md:my-5;
}
</style>
