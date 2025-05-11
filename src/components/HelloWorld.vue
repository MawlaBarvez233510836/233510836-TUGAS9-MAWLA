<template>
  <div>
    <h2>{{ title }}</h2>
    <p>{{ content }}</p>
  </div>
</template>

<script setup>
const props = defineProps({
  title: String,
  content: String
})
</script>

<style scoped>
h2 {
  color: #2c3e50;
}
p {
  font-size: 16px;
}
</style>
