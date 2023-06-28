<template>
 <v-app>
   <SideBar @selectOption="onSelectOption"/>
   <v-main>
     <!-- CARDS -->
    <ImageGallery :isWithColor="isWithColor" />
  </v-main>
 </v-app>
</template>

<script setup>
import ImageGallery from './components/ImageGallery.vue';
import SideBar from './components/SideBar.vue'
import { ref } from 'vue';

const isWithColor = ref(true)
const onSelectOption = (isColor) => {
  isWithColor.value =isColor
}
</script>

