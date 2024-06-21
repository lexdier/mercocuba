<script setup lang="ts">
import carousel from '@/public/assets/images/carousel.png'
</script>

<template>
  <v-row>
    <v-col cols="12">
      <v-carousel hide-delimiters class="h-100 w-100">
        <v-carousel-item
            :src="carousel"
        />

        <v-carousel-item
            :src="carousel"
        />

        <v-carousel-item
            :src="carousel"
        />
      </v-carousel>
    </v-col>
  </v-row>

  <v-row class="py-5">
    <v-col cols="12" class="text-center">
      <div class="flex flex-column">
        <span class="text-lg-h2 text-blue">BIENVENIDO A NUESTRA TIENDA</span>

        <div class="pt-5 d-flex justify-center">
          <v-btn class="me-5" color="blue">
            <span>Mas vendidos</span>
          </v-btn>

          <v-btn  color="blue">
            <span>Mas vistos</span>
          </v-btn>
        </div>
      </div>
    </v-col>
  </v-row>
</template>