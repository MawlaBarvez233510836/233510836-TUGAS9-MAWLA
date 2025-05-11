<template>
  <div class="hello">
    <h2>Ini dari HelloWorld.vue</h2>
    <slot></slot> <!-- Slot default -->
  </div>
</template>

<script>
export default {
  name: "HelloWorld"
};
</script>

<style scoped>
.hello {
  border: 2px solid #42b983;
  padding: 16px;
  margin: 16px;
}
</style>
