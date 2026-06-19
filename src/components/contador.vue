<template>
  <h1>HOLA MUNDO!</h1>
  <h2>
    Contador: <span>{{ contador }}</span>
  </h2>
  <button @click="aumentar">Aumentar</button>
  <button @click="disminuir">Disminuir</button>
</template>

<script setup>
import { ref } from 'vue'
const contador = ref(0)

const aumentar = () => {
  contador.value++
}

const disminuir = () => {
  contador.value--
}
</script>

<style scoped>
span {
  color: red;
}
</style>
