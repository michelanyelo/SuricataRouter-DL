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

<style scoped>
.app-container {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

.main-content {
  flex: 1;
  padding: 20px;
}
</style>
