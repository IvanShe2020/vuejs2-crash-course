<template>
  <div>
    <ul>
      <TodoItem
          v-for="todo of ArrayTodos"
          :key="todo"
          v-bind:todo="todo"
      ></TodoItem>
    </ul>
  </div>
</template>

<script>
import TodoItem from '@/components/todoItem'
export default {
  props: ['ArrayTodos'],
  components: {
    TodoItem
  }
}
</script>

<style scoped>
  ul {
    list-style: none;
    margin: 0;
    padding: 0;
  }
</style>