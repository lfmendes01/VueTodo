
import TodoItem from './TodoItem.vue';

<template>
    <TodoItem v-for="todo in $store.state.todos"
    :key="todo.id" :todo="todo"/>
</template>

<script>
import TodoItem from '@/components/TodoItem.vue';


export default {
    name: "App",
    components: { TodoItem }
}
</script>