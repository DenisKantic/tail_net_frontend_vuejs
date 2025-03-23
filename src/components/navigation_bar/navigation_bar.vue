<template>
  <v-app-bar style="padding: 0 18rem" elevation="4" color="info">
    <v-img src="/src/assets/logo.png" max-width="60" alt="logo"></v-img>
    <v-text-field placeholder="search" variant="outlined" class="pt-4 ml-4"></v-text-field>
    <v-spacer></v-spacer>
    <p class="d-flex flex-column items-center justify-center text-body-2 mr-4">
      <v-icon class="mx-auto" size="25">mdi-home</v-icon>
      Home
    </p>

    <p class="d-flex flex-column items-center justify-center text-body-2 mr-4">
      <v-icon class="mx-auto" size="25">mdi-chat</v-icon>
      Messaging
    </p>
    <p class="d-flex flex-column items-center justify-center text-body-2">
      <v-icon class="mx-auto" size="25">mdi-bell</v-icon>
      Notifications
    </p>
  </v-app-bar>
</template>

<script lang="ts"></script>
