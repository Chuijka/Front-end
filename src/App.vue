<template>
  <header>
    <TheHeader/>
  </header>
  <main>
    <TheProduct title="Puma" price="120$"/>
    <TheProduct title="Nike" price="130$"/>
    <TheProduct title="Nike" price="110$"/>
    <TheProduct title="Adidas" price="115$"/>
    <TheProduct title="Adidas" price="115$"/>
    <TheProduct title="Adidas" price="115$"/>
    <TheProduct title="Adidas" price="115$"/>
  </main>
  <footer>
    <TheFooter/>
  </footer>
</template>

<script setup>
import TheHeader from "./component/TheHeader.vue";
import TheFooter from "./component/TheFooter.vue";
import TheProduct from "./component/TheProduct.vue";

</script>

<style>
body {
  background: #313131;
  color: white;
  font-family: Arial, serif;
  font-size: 20px;
}

footer{
  margin: 30px;
}

</style>
