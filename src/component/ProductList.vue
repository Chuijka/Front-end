<script setup>
import TheProduct from "./TheProduct.vue";

const onClickAdd = () => {
  alert('Add!')
}
const onClickFavorite = () => {
  alert('Add!')
}
</script>

<template>
  <div class="grid grid-cols-4 gap-4">
    <TheProduct
        title="Puma"
        :price="120"
        imageUrl="src/assets/Shoes/sneakers-1.jpg"
        :onClickAdd="onClickAdd"
        :onClickFavorite="onClickFavorite"
    />

  </div>
</template>

<style scoped>

</style>