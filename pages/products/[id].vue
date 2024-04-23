<template>
  <div>
    <h2>Products</h2>
    <p>Product details for {{ id }}</p>

    <p>
      Lorem ipsum, dolor sit amet consectetur adipisicing elit. Dignissimos
      cupiditate, eaque obcaecati, officia accusantium, vero possimus placeat
      harum optio fugiat excepturi eos itaque. Quos dolorem dignissimos quasi
      quam voluptates. Minima?
    </p>
  </div>
</template>

<script setup>
const { id } = useRoute().params;
</script>
<style scoped>
h2 {
  margin-bottom: 20px;
  font-size: 36px;
}
p {
  margin: 20px 0;
}
</style>
