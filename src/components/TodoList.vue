<template>
    <div class="todolist-holder">
        <TodoItem v-for="(todo,i) in todos" :key="i" :todo="todo"  />
    </div>
</template>

<script setup lang="ts">
import { todos } from '@/mock/todos';
import TodoItem from './TodoItem.vue';
</script>

<style scoped>

.todolist-holder {
    margin: 40px auto;
    width: 80%;
   
}
</style>