<template>
  <div>
    <h1>Dipesh Vue Work</h1>
    <TodoList/>
  </div>
</template>

<script>
import TodoList from './components/TodoList.vue';
export default {
  name:"App",
  components:{
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