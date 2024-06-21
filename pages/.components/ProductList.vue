<script setup lang="ts">

import ProductCard from "~/pages/.components/ProductCard.vue";
</script>

<template>
  <v-row>
    <template v-for="(index, item) in 10" :key="index">
      <v-col lg="3" sm="6">
        <ProductCard/>
      </v-col>
    </template>
  </v-row>

  <v-row class="mt-5">
    <v-col class="text-center">
      <v-btn rounded="circle" color="blue" size="100">
        <v-icon size="50" icon="mdi-arrow-u-right-top"/>
      </v-btn>
    </v-col>
  </v-row>
</template>