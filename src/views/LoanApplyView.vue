<script lang="ts">
import { defineComponent } from 'vue'

import NavHeader from '@/components/Nav-Header.vue'
import LoanForm from '../components/Loan-Form.vue'

export default defineComponent({
  components: {
    NavHeader,
    LoanForm
  },
  data() {
    return {
      message: 'Apply'
    }
  }
})
</script>
<template>
  <div class="w-full flex flex-col">
    <NavHeader :greetingMessage="message" />
    <LoanForm />
  </div>
</template>

<style></style>
