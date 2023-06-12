<template>
    <h1>Hello Todo List</h1>
</template>

<script>
export default {
    data(){
        return{
            todos: [
                { todoString: "go to gym", completed: true },
                { todoString: "find some to mall", completed: false },
                { todoString: "publish that video", completed: false },
                { todoString: "get a job", completed: true },
            ]
        }
    },
    methods: {
        addTodo(newTodo){
            this.todos.push({
                todoString: newTodo,
                completed: false
            })
        },

        toggleTodo(todo){
            todo.completed = !todo.completed
        },

        editTodo(todo, newTodoString){
            todo.todoString = newTodoString
        },
        deleteTodo(deleteTodo){
            this.todos = this.todos.filter((todo) => todo !== deleteTodo)
        }
    }
}
</script>

<style>

</style>