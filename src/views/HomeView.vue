<template>
  <div class="w-full flex flex-col">
    <!-- Use the HomeLanding component here -->
    <HomeLanding />
    <LoanType />
    <AboutUs />
    <WhyUs />
    <LatestNews />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import HomeLanding from '@/components/Home-Landing.vue' // Make sure the path is correct
import LoanType from '@/components/Loan-type.vue'
import AboutUs from '@/components/About-us.vue'
import WhyUs from '@/components/Why-us.vue'
import LatestNews from '@/components/Latest-News.vue'

export default defineComponent({
  components: {
    HomeLanding,
    LoanType,
    AboutUs,
    WhyUs,
    LatestNews
  }
})
</script>

<style></style>
