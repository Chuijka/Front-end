<script setup>

import TheClicker from "./TheClicker.vue";

defineProps({
    title: String,
    price: Number
})

</script>

<template>
  <div class="product-block">
    <div class="product">
      <h2>Product: {{ title }}</h2>
      <h3>Price: {{ price }}</h3>
    </div>
    <div class="clicker">
      <TheClicker/>
    </div>
  </div>
</template>

<style scoped>

.product-block {
  border: 1px solid black;
  padding: 10px;
  margin-bottom: 10px;
  height: 150px;
}
.product{
  float: left;
}
.clicker{
  float: right;
}
</style>