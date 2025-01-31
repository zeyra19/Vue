<template lang="">
    <div v-for="todo in todos" :key="todo.key">
        {{todo.title}} - {{todo.completed}}
    </div>
</template>

<script setup lang="ts">
import {ref, onMounted} from "vue";

interface Todo {
    id: number
    userId: number
    title: string
    completed: boolean
}

    const todos = ref<Todo[]>([])

    onMounted(async() => {
        try {
            const response = await fetch("https://jsonplaceholder.typicode.com/todos/")
            const data: Todo[] = await response.json();
            todos.value = data
        } catch (error) {
            console.log(error)
        }
    })


</script>

<style scoped>
</style>