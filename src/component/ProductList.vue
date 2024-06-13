<script setup>
import TheProduct from "./TheProduct.vue";
</script>

<template>
  <div class="grid grid-cols-4 gap-4">
    <TheProduct title="Puma" :price="120" imageUrl="../assets/Shoes/sneakers-1.jpg"/>
    <TheProduct title="Nike" :price="130"/>
    <TheProduct title="Nike" :price="110"/>
    <TheProduct title="Adidas" :price="115"/>
  </div>
</template>

<style scoped>

</style>