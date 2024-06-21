<script setup lang="ts">
import logo from '../public/assets/images/logo.jpg'
</script>

<template>
  <nav class="bg-black">
    <v-container>
      <v-row align="center">
        <v-col cols="3" class="d-flex align-center">
          <v-img class="w-25" height="150" :src="logo"/>
        </v-col>

        <v-col cols="8" class="d-flex align-center">
          <v-text-field variant="solo" placeholder="Buscar productos...">
            <template v-slot:append class="ma-0 pa-0">
              <v-icon size="60" icon="mdi-magnify"></v-icon>
            </template>
          </v-text-field>
        </v-col>
      </v-row>
    </v-container>
  </nav>

  <nav class="border-b elevation-2">
    <v-container>
      <v-row>
        <v-col cols="9">
          <v-btn icon="mdi-home" class="rounded" color="blue"/>
        </v-col>

        <v-col class="d-flex justify-space-between">
          <v-btn size="x-large" icon="mdi-account-circle" variant="plain"/>
          <v-btn size="x-large" icon="mdi-heart" variant="plain"/>
          <v-btn size="x-large" icon="mdi-cart" variant="plain"/>
          <v-btn size="x-large" icon="mdi-menu" variant="plain"/>
        </v-col>
      </v-row>
    </v-container>
  </nav>
</template>
