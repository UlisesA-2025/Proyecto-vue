<script setup>
import { useCounterStore } from '../stores/counter' // Importa el store

const counter = useCounterStore() // Usa el store en el componente
</script>

<template>
  <div style="text-align: center; margin-top: 20px;">
    <h2>Contador</h2>
    <p style="font-size: 24px;">Valor actual: {{ counter.count }}</p>
    <button @click="counter.increment">Incrementar</button>
  </div>
</template>
