<script setup>
defineProps({
    tittle: String,
    count: Number
})

const emit = defineEmits(['increment'])
</script>

<template>
    <div class="card">
        <h2>[{ title }]</h2>
        <p>Valor: {{ count }}</p>
        <button @click="emit('increment')">
            incrementar
        </button>
    </div>
</template>

<style scoped>
.card{
    border: 1px solid #ccc;
    padding: 20px;
    border-radius: 8px;
    width: 250px;
}
button {
  margin-top: 10px;
}
</style>