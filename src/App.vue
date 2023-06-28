<template>
 <v-app>
<SideBar />
  <v-main>
    <!-- CARDS -->
    <ImageGallery />
  </v-main>
 </v-app>
</template>

<script setup>
import ImageGallery from './components/ImageGallery.vue';
import SideBar from './components/SideBar.vue'
</script>

