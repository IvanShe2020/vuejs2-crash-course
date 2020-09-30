<template>
  <div id="app">
    <h1>{{ tittle }}</h1>
    <hr>
    <TodoList
        v-bind:ArrayTodos="ArrayTodos"
    ></TodoList>
  </div>
</template>

<script>
import TodoList from '@/components/todoList'
export default {
  name: 'App',
  components: {
    TodoList
  },
  data() {
    return {
      tittle: 'Todo application',
      ArrayTodos:[
        {id:1, title:'Купить хлебушка',complete: false},
        {id:2, title:'Купить car',complete: false},
        {id:3, title:'Купить multivarka',complete: false},
      ]
    }
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
