<template>
    <div class="todo-item-holder">
        <input class="checkbox-input" type="checkbox" id="checkbox" v-model="status" />
        <label :class="{ 'complete-todo': status }" for="checkbox">{{ todo.Title }}</label>
    </div>
</template>

<script setup lang="ts">
import type { Todo } from '@/types/todo';
import { ref } from 'vue';
const props = defineProps<
    { todo: Todo }
>()
const status = ref<boolean>(props.todo.Completed)


</script>

<style scoped>
.todo-item-holder {
    border-bottom: 1px solid rgb(105, 126, 228);;
    padding: 30px 0;
    font-size: 20px;
    display: flex;
    flex-direction: row;
   align-items: center;
}

.todo-item-holder .todo-title {
    margin-left: 30px;
}

.complete-todo {
    text-decoration: line-through;
}

.checkbox-input {
    width: 20px;
    margin: 20px;
    padding: 10px;

    height: 40px;
}
</style>