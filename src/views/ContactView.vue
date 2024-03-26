<template>
  <div class="w-full flex flex-col">
    <NavHeader :greetingMessage="message" />
    <ContactMaps />
    <ContactForm />
  </div>
</template>
<script lang="ts">
import { defineComponent } from 'vue'

import NavHeader from '@/components/Nav-Header.vue'
import ContactMaps from '@/components/Contact-Maps.vue'
import ContactForm from '@/components/Contact-Form.vue'

export default defineComponent({
  components: {
    NavHeader,
    ContactMaps,
    ContactForm
  },
  data() {
    return {
      message: 'Contact Us'
    }
  }
})
</script>

<style></style>
