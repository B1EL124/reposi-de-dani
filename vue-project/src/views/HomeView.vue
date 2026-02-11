<script setup>
import { ref } from 'vue'

const count = ref(0)

function incrementar() {
  count.value++
}
</script>

<template>
  <div style="padding: 40px">
    <h1>Projeto Vue 3 - Aula Prática</h1>
    
    <p>Contador: {{ count }}</p>
    
    <button @click="incrementar">
      Incrementar
    </button>
  </div>
</template>