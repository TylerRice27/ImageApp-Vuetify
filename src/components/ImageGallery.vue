<template>
    <v-card class="mx-5 my-2 pa-3">
    <v-row >
        <v-col :key="n" v-for="n in 198" cols="6" sm="4" md="2">
            <v-hover
            v-slot="{ isHovering, props }"
            close-delay="200"
          >
            <v-card  :elevation="isHovering ? 16 : 2"
              :class="{ 'on-hover': isHovering }" v-bind:="props">
             <v-img :src="`https://picsum.photos/500/300?image=${n * 5 + 10}${colorProp.isWithColor ? '' : '&grayscale'}`"
             :lazy-src="`https://picsum.photos/500/6?image=${n * 5 + 10}${colorProp.isWithColor ? '' : '&grayscale'}`"
             aspect-ratio="1" cover>
            <template v-slot:placeholder>
              <v-row
                class="fill-height ma-0"
                align="center"
                justify="center"
              >
                <v-progress-circular
                  indeterminate
                  color="grey-lighten-5"
                ></v-progress-circular>
                </v-row>
            </template>
            </v-img>
            </v-card>
            </v-hover>
        </v-col>
    </v-row>
     </v-card>
</template>


<script setup>
import { defineProps } from 'vue';

const colorProp = defineProps(["isWithColor"])
</script>