<script setup>
import Navbar from './components/NavbarComponent.vue'
import Footerbar from './components/FooterbarComponent.vue'
</script>

<template>
  <div class="min-h-screen flex flex-col bg-gray-700">
    <Navbar/>
    <main class="flex-grow container mx-auto px-4 py-6">
      <router-view></router-view>
    </main>
    <Footerbar/>
  </div>
</template>