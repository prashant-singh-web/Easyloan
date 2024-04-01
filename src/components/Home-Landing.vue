<template>
  <div class="w-full h-fit relative text-black">
    <div class="w-full absolute top-0 left-0 h-full">
      <div class="absolute w-full h-full bg-sky-500/40 z-[1]"></div>
      <img src="../assets/home.jpg" alt="home" class="w-full h-full" />
    </div>
    <div
      class="w-[90%] lg:w-3/4 mt-20 mx-auto py-10 md:py-20 h-full grid grid-cols-1 place-items-center gap-5 md:grid-cols-2"
    >
      <div class="flex flex-col mx-auto z-[5] h-full">
        <h4 class="h4-header">The simple</h4>
        <h4 class="h4-header">online home</h4>
        <h4 class="h4-header border-b-4 pb-4 border-white w-fit">loan.</h4>
        <p class="text-lg md:text-2xl mt-4 text-white font-medium">
          Financial uncertainty is hard on employees, and causes even.
        </p>
        <RouterLink
          to="/services"
          class="text-lg mt-6 font-medium border-2 border-white px-7 py-3 text-white w-fit"
        >
          Our Services
        </RouterLink>
      </div>
      <div
        class="w-full flex-col bg-white z-[5] m-5 p-4 text-center my-auto hidden sm:flex sm:w-3/4 md:w-full"
      >
        <h2 class="text-2xl font-bold text-sky-800">How much you want?</h2>
        <p class="text-sm font-medium">We provide online instant loan.</p>
        <hr class="w-16 h-1 bg-sky-500 mx-auto my-5" />
        <div class="w-full flex flex-col text-left relative mt-5">
          <label for="amount" class="text-sm font-medium my-2">Amount you want</label>
          <input
            @change="getAmount"
            type="text"
            id="amount"
            placeholder="Select Amount"
            class="w-full border-[1.5px] border-black p-2 focus-within:border-sky-500 outline-none"
          />
          <div class="absolute right-2 bottom-2">
            <FaHome class="text-xl text-black" />
          </div>
        </div>
        <div class="w-full flex flex-col text-left relative">
          <label for="month" class="text-sm font-medium my-2">Month</label>
          <div class="relative z-[2]" @click="toggleDropdown">
            <input
              type="text"
              id="month"
              placeholder="Select"
              :value="monthValue"
              disabled
              class="w-full relative z-[-1] border-[1.5px] border-gray-500 p-2 outline-none"
            />

            <button @click="toggleDropdown" class="absolute right-2 top-2">
              <i
                :class="{
                  'fa-solid fa-angle-down': !showDropdown,
                  'fa-solid fa-angle-up': showDropdown,
                }"
              ></i>
            </button>

            <div
              @click="toggleDropdown"
              v-if="showDropdown"
              class="origin-top-left absolute left-0 w-full rounded shadow bg-white mt-1"
            >
              <p @click="getMonth('3 month')" class="select-button">3 months</p>
              <p @click="getMonth('6 month')" class="select-button">6 months</p>
              <p @click="getMonth('3 weeks')" class="select-button">3 weeks</p>
              <!-- ... more options ... -->
            </div>
          </div>
        </div>
        <p class="text-sm font-medium text-left my-2 text-gray-900/80">
          You have to pay : <span>${{ price }}</span>
        </p>
        <button
          class="py-2 text-sm font-semibold text-white bg-sky-500 rounded shadow-sm"
        >
          Apply
        </button>
        <p class="text-base text-gray-900/70 font-semibold my-3">
          we provide online instant cash loans.
        </p>
      </div>
    </div>
  </div>
</template>
<script lang="ts">
import { defineComponent, ref } from "vue";

export default defineComponent({
  data() {
    return {
      showDropdown: ref(false),
      monthValue: ref("select month"),
      price: ref(0),
    };
  },
  methods: {
    toggleDropdown(): void {
      this.showDropdown = !this.showDropdown;
    },

    getMonth(value: string): void {
      this.monthValue = value;
      this.showDropdown = !this.showDropdown;
    },
    getAmount(e: any) {
      this.price = e.target.value;
    },
  },
});
</script>

<style>
.select-button {
  @apply block px-4 py-2 text-gray-700 hover:bg-gray-100 focus:outline-none cursor-pointer;
}
.h4-header {
  @apply text-2xl sm:text-4xl md:text-5xl lg:text-6xl font-bold text-white;
}
</style>
