<!--option API-->
<script>

export default {
  data() {
    return {
      count: 0
    }
  },
  methods: {
    add() {
      this.count++
    },
    minus() {
      this.count--
    }
  }
}

</script>

<!--composition API-->
<script setup>
import {ref} from "vue";

const count = ref(0)

function add() {
  count.value++
  console.log(count)
}

function minus() {
  count.value--
  console.log(count)
}

function updateText(event){
      count.value = Number(event.target.value)
}
</script>

<template>
  <div>
    <h1>{{ count }}</h1>
    <button @click="add">+</button>
    <button @click="minus">-</button>
    <!--    <button @click="count++">+</button>  "Різновид виводу додавання"  -->
    <!--    <button @click="count--">-</button>  "Різновид виводу віднімання"  -->
<!--    <input v-model="count">  "Модель для оновлення лічильника"  -->
<!--    <input @input="updateText">  "Виконується коли є ф-ція updateText"  -->
    <input @keyup.enter="updateText"  />

  </div>
</template>

<style scoped>
div {
  text-align: center;
}
input{
  width: 50px;
}
</style>