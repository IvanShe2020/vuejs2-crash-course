<template>
  <div id="app">
    <h1>Todo aplication</h1>
    <hr>
    <tL></tL>
  </div>
</template>

<script>
import tL from '@/components/todoList'
export default {
  name: 'App',
  components: {
    tL
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
