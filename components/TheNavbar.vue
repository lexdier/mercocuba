<script setup lang="ts">
import logo from '../public/assets/images/logo.jpg'

const items = ['text', 'text', 'text longer', 'text even more longer']
</script>

<template>
  <nav class="bg-black">
    <v-container>
      <v-row align="center">
        <v-col lg="3" class="d-flex align-center">
          <v-img class="w-25" height="150" :src="logo"/>
        </v-col>

        <v-col lg="8" class="d-flex align-center">
          <v-text-field
              hide-details
              label="Buscar productos"
              variant="solo"
              class="w-100"
          >
            <template v-slot:prepend>
              <v-select
                  variant="solo"
                  :items="items"
              >
                <template v-slot:label clas="w-100">
                  Todos
                </template>
              </v-select>
            </template>

            <template v-slot:append>
              <v-icon icon="mdi-magnify" class="bg-blue rounded" size="80"/>
            </template>
          </v-text-field>
        </v-col>
      </v-row>
    </v-container>
  </nav>

  <nav class="border-b elevation-2">
    <v-container>
      <v-row align="center">
        <v-col>
          <v-btn icon="mdi-home" class="rounded" color="blue"/>
        </v-col>

        <v-col cols="auto" class="d-flex justify-space-between">
          <v-btn size="x-large" icon="mdi-account-circle" variant="plain"/>
          <v-btn size="x-large" icon="mdi-heart" variant="plain"/>
          <v-btn size="x-large" icon="mdi-cart" variant="plain"/>
          <v-btn size="x-large" icon="mdi-menu" variant="plain"/>
        </v-col>
      </v-row>
    </v-container>
  </nav>
</template>
