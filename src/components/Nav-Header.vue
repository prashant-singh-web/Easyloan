<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  props: {
    greetingMessage: {
      type: String,
      required: true
    }
  }
})
</script>
<template>
  <div class="w-full bg-sky-600 grid place-items-center">
    <p class="text-4xl font-semibold text-white py-20">{{ greetingMessage }}</p>
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
