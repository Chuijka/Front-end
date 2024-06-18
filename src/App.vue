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

        <ProductList/>

      </div>

    </main>

    <footer class="flex justify-between border-slate-200 pb-5">
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
  background: linear-gradient(to right, rgba(252, 109, 72, 0.5), rgba(250, 183, 88, 0.7));
  color: #000000;
  font-family: Arial, serif;
  font-size: 20px;
}

footer {
  margin: 30px;
}

</style>
