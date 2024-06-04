<script setup>
import { RouterView } from 'vue-router'
import NavC from '@/components/NavC.vue'
import FooterC from '@/components/FooterC.vue'
</script>

<template>
  <NavC />

  <RouterView />

  <FooterC />
</template>
