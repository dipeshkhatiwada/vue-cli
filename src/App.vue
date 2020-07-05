<template>
  <div>
    <h1>helloNepal</h1>
    <TodoList/>
  </div>
</template>

<script>
import TodoList from './components/todoList.hljs-value';
export default {
  name:"App",
  Components:{
    TodoList
    }
};
</script>

<style>
body{
  background-color: rgb(26,26,26);
  color: aliceblue;
}

</style>