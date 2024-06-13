<script setup>
import DrawerHead from "./DrawerHead.vue";
import ProductListInDrawer from "./ProductListInDrawer.vue";
</script>

<template>
  <div class="fixed top-0 left-0 h-full w-full bg-black z-10 opacity-80"></div>
  <div class="bg-white w-96 fixed top-0 right-0 h-full z-20 p-8">
    <DrawerHead/>
    <ProductListInDrawer/>

    <div class="flex flex-col gap-4 my-8">
      <div class="flex gap-2 mb-4">
        <span>Result:</span>
        <div class="flex-1 border-b border-slate-200"></div>
        <b>120 $</b>
      </div>

      <button
          disabled=""
          class="disabled:bg-slate-400 transition bg-lime-500 w-full rounded-xl py-1 text-white hover:bg-lime-600 active:bg-lime-700 cursor-pointer">
        To order
      </button>
    </div>
  </div>
</template>

<style scoped>

</style>