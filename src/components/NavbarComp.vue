<template>
  <nav class="navbar navbar-expand-lg navbar-light">
    <div class="container px-4">
      <RouterLink class="navbar-brand" to="/">
        <img src="../assets/logo.png" alt="logo de suricata" />
      </RouterLink>
      <button class="navbar-toggler navbar-dark border-light" type="button" data-bs-toggle="collapse"
        data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false"
        aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item">
            <RouterLink class="nav-link text-light" :to="{ name: 'home' }">Inicio</RouterLink>
          </li>
          <li class="nav-item">
            <RouterLink class="nav-link text-light" :to="{ name: 'productos' }">Productos</RouterLink>
          </li>
          <li class="nav-item">
            <RouterLink class="nav-link text-light" :to="{ name: 'contacto' }">Contacto</RouterLink>
          </li>
          <li class="nav-item">
            <RouterLink class="nav-link text-light" :to="{ name: 'about' }">Acerca de</RouterLink>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script setup>
import { RouterLink } from 'vue-router'
</script>

<style scoped></style>
