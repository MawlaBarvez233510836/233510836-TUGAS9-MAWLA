<template>
  <div>
    <h2>{{ title }}</h2>
    <p>{{ content }}</p>
    <button @click="handleClick">Kirim Event ke Parent</button>
  </div>
</template>

<script setup>
const props = defineProps({
  title: String,
  content: String
})

const emit = defineEmits(['notify'])

function handleClick() {
  emit('notify', 'Halo dari komponen anak!')
}
</script>

<style scoped>
h2 {
  color: #2c3e50;
}
p {
  font-size: 16px;
}
button {
  margin-top: 10px;
  padding: 6px 12px;
  background-color: #42b983;
  border: none;
  color: white;
  cursor: pointer;
}
</style>
