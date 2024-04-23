<template>
  <div>
    <h2 class="mb-4">Product # {{ id }}</h2>

    <p>{{ product.title }}</p>
    <p>€ {{ product.price }}</p>
    <p># {{ product.id }}</p>
  </div>
</template>

<script setup>
const { id } = useRoute().params;
const uri = 'https://fakestoreapi.com/products/' + id;

// fetch product
const { data: product } = await useFetch(uri, { key: id });

definePageMeta({
  layout: 'products',
});
</script>

<style scoped></style>
