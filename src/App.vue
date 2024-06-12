<template>
  <div>
    <TheHeader/>
    <main>
      <TheProduct title="Shoes Puma" price="120$"/>
      <TheProduct/>
      <TheProduct/>
      <TheProduct/>
    </main>
    <TheFooter/>
  </div>
</template>

<script setup>
import TheHeader from "@/component/TheHeader.vue";
import TheFooter from "@/component/TheFooter.vue";
import TheProduct from "@/component/TheProduct.vue";

</script>

<style>
  body{
    background: #313131;
    color: white;
    font-family: Arial,serif;
    font-size: 20px;
  }

</style>
