<script setup lang="ts">
import TheNavbar from "~/components/TheNavbar.vue";
import TheCarousel from "~/pages/.components/Carousel.vue";
import ProductList from "~/pages/.components/ProductList.vue";
</script>

<template>
  <NuxtLayout>
    <section class="py-5">
      <TheCarousel/>
    </section>

    <section>
      <ProductList/>
    </section>
  </NuxtLayout>
</template>
