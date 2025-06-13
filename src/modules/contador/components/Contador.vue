<template>
  <h1>Hola mundo</h1>
  <p>{{ contador }}</p>
  <button @click="incrementar">Incrementar</button>
  <button @click="restar">Restar</button>
</template>

<script setup>
  import {ref} from "vue";
  const contador = ref(0);

  const incrementar = () =>{
    contador.value++;
  }
  const restar = () =>{
    contador.value--;
  }
</script>

<style scoped>
  p{
    color: red;
  }
</style>
