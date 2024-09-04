<template>
  <div class="app-container">
    <Navbar />
    <main class="main-content">
      <RouterView />
    </main>
    <MediosPago />
    <FooterMenu />
  </div>
</template>

<script setup>
import { RouterView } from 'vue-router'
import Navbar from '@/components/NavbarComp.vue'
import FooterMenu from '@/components/FooterComp.vue'
import MediosPago from '@/components/MediosPago.vue'
</script>

<style scoped></style>
