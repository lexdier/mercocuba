<script setup lang="ts">
import carousel from '@/public/assets/images/carousel.png'
</script>

<template>
  <v-row>
    <v-col cols="12">
      <v-carousel hide-delimiters class="h-100">
        <v-carousel-item
            height="800"
            :src="carousel"
        />

        <v-carousel-item
            height="800"
            :src="carousel"
        />

        <v-carousel-item
            height="800"
            :src="carousel"
        />
      </v-carousel>
    </v-col>
  </v-row>

  <v-row>
    <v-col cols="12" class="text-center">
      <div class="flex flex-column">
        <h2>BIENVENIDO A NUESTRA TIENDA</h2>

        <div class="pt-5">
          <v-btn class="me-5" size="large">
            <span>Mas vendidos</span>
          </v-btn>

          <v-btn size="large">
            <span>Mas vistos</span>
          </v-btn>
        </div>
      </div>
    </v-col>
  </v-row>
</template>