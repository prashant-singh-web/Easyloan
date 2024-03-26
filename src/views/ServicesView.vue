<template>
  <div class="w-full flex flex-col">
    <NavHeader :greetingMessage="message" />
    <LoanType />
    <LoanStep />
  </div>
</template>
<script lang="ts">
import { defineComponent } from 'vue'

import LoanType from '@/components/Loan-type.vue'
import LoanStep from '@/components/Loan-Steps.vue'
import NavHeader from '@/components/Nav-Header.vue'

export default defineComponent({
  components: {
    LoanType,
    LoanStep,
    NavHeader
  },
  data() {
    return {
      message: 'Services'
    }
  }
})
</script>

<style></style>
