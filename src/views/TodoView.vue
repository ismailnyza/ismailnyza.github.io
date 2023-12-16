<script lang="ts" setup>
import SingleTodo from "@/components/singleTodo.vue";

// move to getting from service
const todos = [
  {
    title: "Todo 1",
    description: "This is the first todo",
    Due: 10 / 10 / 2021,
    isChecked: false,
  },
  {
    title: "Todo 2",
    description: "This is the second todo",
    Due: 9 / 10 / 2021,
    isChecked: false,
  },
  {
    title: "Todo 3",
    description: "This is the third todo",
    Due: 10 / 10 / 2021,
    isChecked: true,
  },
  // Add more todos as needed
];
</script>

<template>
  <h2>Ismail's Impossible List :D</h2>
  <div class="grid grid-cols-6 gap-4">
    <div>
      <SingleTodo v-for="(todo, index) in todos" :key="index" :description="todo.description"
                  :due="todo.Due" :is-checked="todo.isChecked" :title="todo.title"/>
    </div>
  </div>
  <button>+ Suggest</button>

</template>

<style scoped>

</style>
