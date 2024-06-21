<script setup lang="ts">
import logo from '../public/assets/images/logo.jpg'

const items = ['text', 'text', 'text longer', 'text even more longer']
</script>

<template>
  <nav class="bg-black">
    <v-container>
      <v-row align="center">
        <v-col lg="3" cols="2" class="d-flex align-center">
          <v-img  min-height="40" max-height="150" :src="logo"/>
        </v-col>

        <v-col lg="9" sm="10" class="d-flex align-center">
          <v-row>
            <v-col lg="2" cols="2">
              <v-select
                  variant="solo"
                  :items="items"
                  label="Todos"
                  bg-color="blue"
                  hide-details
              />
            </v-col>

            <v-col lg="8" cols="6">
              <v-text-field
                  hide-details
                  label="Buscar productos"
                  variant="solo"
              >
              </v-text-field>
            </v-col>

            <v-col lg="2" cols="1">
              <v-btn class="h-100" color="blue">
                <v-icon icon="mdi-magnify" size="auto"/>
              </v-btn>
            </v-col>
          </v-row>
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
