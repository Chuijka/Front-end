<template>
  <div class="bg-white w-4/5 rounded-3xl shadow-xl m-auto my-4">
    <header class="flex justify-between border-b border-slate-200 px-8 py-5">
      <TheHeader/>
    </header>
    <main>
      <div class="p-10">
        <h2 class="text-3xl font-bold m-2">All Shoes</h2>
        <ProductList/>
      </div>

    </main>
    <footer>
      <TheFooter/>
    </footer>
  </div>
</template>

<script setup>
import TheHeader from "./component/TheHeader.vue";
import TheFooter from "./component/TheFooter.vue";
import ProductList from "./component/ProductList.vue";

</script>

<style>
body {
  background-color: rgb(110, 110, 110);
  color: #000000;
  font-family: Arial, serif;
  font-size: 20px;
}

footer{
  margin: 30px;
}

</style>
