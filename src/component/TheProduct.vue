<script setup>

defineProps({
  title: String,
  price: Number,
  imageUrl: String,
  isFavorite: Boolean,
  isAdded: Boolean,
  onClickAdd: Function,
  onClickFavorite: Function
})

</script>

<template>
  <div>
    <div class="relative m-5 border scale-100 rounded-3xl p-8 cursor-pointer transition hover:shadow-xl hover:-translate-y-1">
      <img :src="!isFavorite ? 'src/assets/like-1.svg' : 'src/assets/like-2.svg'"
           alt="Like 1"
           class="absolute top-8 left-8"
           @click="onClickFavorite"
      >
      <img :src="imageUrl" alt="Sneaker">
      <p class="mt-2">{{ title }}</p>

      <div class="flex justify-between mt-5">
        <div class="flex flex-col">
          <span style="color: #7a7a7a">price:</span>
          <b>{{ price }}$</b>
        </div>
        <img :src="!isAdded ? 'src/assets/plus.svg' : 'src/assets/checked.svg'"
             alt="plus"
             @click="onClickAdd"
        >
      </div>
    </div>

  </div>
</template>

<style scoped>

</style>