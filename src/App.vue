<template>
  <Navbar />

  <router-view />

  <medios-pago />
  <FooterMenu />
</template>

<script>
import Navbar from '@/components/NavbarComp.vue'
import FooterMenu from '@/components/FooterComp.vue'
import MediosPago from '@/components/MediosPago.vue'

export default {
  name: 'HomeView',
  components: {
    Navbar,
    FooterMenu,
    MediosPago
  }
}
</script>
