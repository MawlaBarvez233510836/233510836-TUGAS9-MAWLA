<template>
  <div id="app">
    <HelloWorld>
      <p>Isi dari slot default. Ini dikirim dari App.vue ke HelloWorld.vue</p>
    </HelloWorld>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  margin-top: 40px;
}
</style>
