<template>
    <v-navigation-drawer expand-on-hover rail>
      <v-list>
              <v-list-item
                prepend-avatar="https://randomuser.me/api/portraits/women/85.jpg"
                title="Tyler Rice"
                subtitle="cool.ty@gmail.com"
              ></v-list-item>
            </v-list>
<v-divider></v-divider>

    <v-list density="compact" nav>
              <v-list-item prepend-icon="mdi-image" title="Color Gallery" value="color" @click="selectOption(true)"></v-list-item>
              <v-list-item prepend-icon="mdi-dialpad" title="Grayscale Gallery" value="gray"  @click="selectOption(false)"></v-list-item>
            </v-list>

    </v-navigation-drawer>
</template>


<script setup>
import { defineEmits } from 'vue';


const emit = defineEmits(['selectOption']) 

const selectOption = (isColor) => {
    emit("selectOption", isColor)
}
</script>

