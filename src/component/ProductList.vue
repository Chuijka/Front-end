<script setup>
import TheProduct from "./TheProduct.vue";

defineProps({
  items: Array
})

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
        v-for="item in items"
        :key="item.id"
        :title="item.name"
        :price="item.price"
        :imageUrl="item.images"
    />

  </div>
</template>

<style scoped>

</style>