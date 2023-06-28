<template>
    <v-navigation-drawer expand-on-hover rail>
      <v-list>
              <v-list-item
                prepend-avatar="https://randomuser.me/api/portraits/women/85.jpg"
                title="Tyler Rice"
                subtitle="cool.ty@gmailcom"
              ></v-list-item>
            </v-list>
<v-divider></v-divider>

    <v-list density="compact" nav>
              <v-list-item prepend-icon="mdi-image" title="Color Gallery" value="color"></v-list-item>
              <v-list-item prepend-icon="mdi-dialpad" title="Grayscale Gallery" value="gray"></v-list-item>
            </v-list>

    </v-navigation-drawer>
</template>

