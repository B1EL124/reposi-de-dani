<script setup>
import { ref } from 'vue'
import CounterCard from '@/components/CounterCard.vue'

const count = ref(0)

function incrementar() {
  count.value++
}
</script>

<template>
  <div style="padding: 40px">
    <h1>Projeto Vue 3 - Componentes</h1>
    
    <CounterCard
      title="Meu contador"
      :count="count"
      @increment="incrementar"
    />
  </div>
</template>