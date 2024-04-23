<template>
    <div>
        <img :src="product.image" alt="product thumb" class="thumb">
        <p class="font-bold text-gray-500 m-4 truncate">{{ product.title }}</p>
    </div>
</template>

<script setup>
    const {product} = defineProps(['product'])
</script>

<style scoped>

</style>