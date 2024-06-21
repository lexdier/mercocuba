<script setup lang="ts">
import product from '@/public/assets/images/product.png'
</script>

<template>
    <v-card class="pa-5">
      <v-row>
        <v-col cols="12" class="d-flex">
          <v-img
              rounded
              :src="product"
              cover
          />
        </v-col>

        <v-col cols="12">
          <div>
            <span class="text-h4">Nombre del producto</span>
          </div>
          <div>
            <span class="text-h5">Descripciónde cada producto...</span>
          </div>
        </v-col>

        <v-col cols="12">
          <div>
            <v-icon icon="mdi-information"/>
            <span>Compra mayor de N elementos</span>
          </div>

          <div>
            <v-rating/>
            <div class="d-flex justify-space-between">
              <span class="text-h5">CUP</span>
              <span> <v-icon size="50" icon="mdi-heart" color="orange"/></span>
            </div>
          </div>
        </v-col>
        <v-col cols="12" class="d-flex justify-end">
          <div class="text-h5 me-2">
            <p class="text-decoration-line-through">0,00</p>
            <p>0,00</p>
          </div>

          <v-icon size="50" icon="mdi-cart-plus" color="orange"/>
        </v-col>
      </v-row>
    </v-card>
</template>
