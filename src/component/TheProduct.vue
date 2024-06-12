<script setup>

import TheClicker from "./TheClicker.vue";

defineProps({
    title: String,
    price: Number
})

</script>

<template>

  <div class="product">
    <h2>Product: {{ title }}</h2>
    <h3>Price: {{ price }}</h3>
<!--    <h2>Product: Puma</h2>-->
<!--    <h3>Price: 120 $</h3>-->
    <div>
      <TheClicker/>
    </div>
  </div>

</template>

<style scoped>

.product {
  border: 1px solid black;
  padding: 10px;
  margin-bottom: 10px;
}
</style>