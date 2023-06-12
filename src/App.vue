<template>
  <div>
    <h1>Hello world!</h1>
    <TodoList/>
  </div>
</template>

<script>

import TodoList from './components/todoList.vue';

export default {
  name: 'App',
  components :{
    TodoList
  }
}
</script>

<style>
body{
  background: rgb(66, 66, 66);
  color: aliceblue;
}
</style>
