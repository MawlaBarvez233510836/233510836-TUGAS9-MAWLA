<script setup>
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <div>
    <h1>Aplikasi Vue Props</h1>

    <HelloWorld 
      title="Judul dari Parent" 
      content="Ini adalah konten yang dikirim dari parent ke komponen anak." 
    />
  </div>
</template>

<style scoped>
h1 {
  color: darkgreen;
  margin-bottom: 20px;
}
</style>
