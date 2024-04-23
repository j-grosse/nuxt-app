<template>
  <div>
    <h2 class="mb-4">Products</h2>
    <div class="grid grid-cols-4 gap-5">
      <div v-for="p in products">
        <ProductCard :product="p"/>
      </div>
    </div>
  </div>
</template>

<script setup>
// composable functions

definePageMeta({
  layout: 'products',
});

// fetch products (destructure data as products)
const { data: products } = await useFetch('https://fakestoreapi.com/products');
</script>

<style scoped></style>
