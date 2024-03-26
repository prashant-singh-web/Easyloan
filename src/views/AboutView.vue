<template>
  <div class="w-full flex flex-col">
    <NavHeader :greetingMessage="message" />
    <AboutUs />
    <WhyUs />
    <LoanStep />
  </div>
</template>
<script lang="ts">
import { defineComponent } from 'vue'

import AboutUs from '@/components/About-us.vue'
import LoanStep from '@/components/Loan-Steps.vue'
import WhyUs from '@/components/Why-us.vue'
import NavHeader from '@/components/Nav-Header.vue'

export default defineComponent({
  components: {
    AboutUs,
    WhyUs,
    LoanStep,
    NavHeader
  },
  data() {
    return {
      message: 'About us'
    }
  }
})
</script>

<style></style>
