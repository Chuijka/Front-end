<template>
  <!--  <TheDrawer/>-->
  <div class="bg-white w-4/5 rounded-3xl shadow-xl m-auto my-4">

    <header class="flex justify-between border-b border-slate-200 px-8 py-5">
      <TheHeader/>
    </header>

    <main class="border-b">
      <div class="p-10">

        <div class="flex justify-between items-center">

          <h2 class="text-3xl font-bold m-2">All Shoes</h2>
          <div class="flex gap-4">
            <div>
              <select class="border border-neutral-300 py-2 px-3 rounded-md outline-none focus:border-neutral-400 transition">
                <option>by name</option>
                <option>from cheap to expensive</option>
                <option>from expensive to cheap</option>
              </select>
            </div>

            <div class="relative">
              <img class="absolute top-3 left-3" src="../src/assets/search.svg" alt="search">
              <input
                  placeholder="search..."
                  class="border border-neutral-300 rounded-md pl-9 pr-2 py-1 outline-none focus:border-neutral-400 transition"
                  type="text">
            </div>
          </div>


        </div>

        <ProductList :items="items" />

      </div>

    </main>

    <footer class="flex justify-between border-slate-200 pb-5">
      <TheFooter/>
    </footer>

  </div>
</template>

<script setup>
import axios from "axios";
import {onMounted, ref} from "vue";

import TheHeader from "./component/TheHeader.vue";
import TheFooter from "./component/TheFooter.vue";
import ProductList from "./component/ProductList.vue";

const items = [
  {
    "brand": "Nike",
    "id": 1,
    "images": "https://hypesneakershop.com.ua/content/images/4/78x78l80nn0/94206165266891.webp",
    "name": "Air Force 1 '07 | CW2288-111, 42.5",
    "stock": 99,
    "price": "$8,600.00"
  },
  {
    "brand": "New Balance",
    "id": 2,
    "images": "https://hypesneakershop.com.ua/content/images/40/78x78l80nn0/71192260999084.webp",
    "name": "990 | U990GR4, 42",
    "stock": 20,
    "price": "$7,599.00"
  }
];

// const items = ref([]);
//
// onMounted(async ()=>{
//   try {
//     const {data} = await axios.get('admin-secret-devlatest')
//
//     // console.log(data)
//     items.value = data;
//   }catch (err){
//     console.log(err)
//   }
// })

</script>

<style>
body {
  background: linear-gradient(to right, rgba(252, 109, 72, 0.5), rgba(250, 183, 88, 0.7));
  color: #000000;
  font-family: Arial, serif;
  font-size: 20px;
}

footer {
  margin: 30px;
}

</style>
