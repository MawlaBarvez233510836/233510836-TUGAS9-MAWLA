<script setup>
import { ref } from 'vue'
import HelloWorld from './components/HelloWorld.vue'

const pesan = ref('')
function tanganiNotifikasi(msg) {
  pesan.value = msg
}
</script>

<template>
  <div>
    <h1>Aplikasi Vue Emits</h1>

    <HelloWorld 
      title="Belajar Emits" 
      content="Klik tombol di bawah untuk kirim event." 
      @notify="tanganiNotifikasi"
    />

    <p v-if="pesan" style="margin-top: 20px; color: red;">
      Pesan dari anak: {{ pesan }}
    </p>
  </div>
</template>

<style scoped>
h1 {
  color: darkgreen;
  margin-bottom: 20px;
}
</style>
