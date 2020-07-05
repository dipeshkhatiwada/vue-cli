<template>
    <h1>hello from todp list</h1>
</template>

<script>
export default {
  data(){
      return{
          todos:[
              {todoString: "make vue", completed:false},
              {todoString: "new vue", completed:true},
              {todoString: "next vue", completed:false},
              {todoString: "old vue", completed:true},
          ]
        }
    },
    methods:{
        addTodo(newTodo){
            this.todos.push({
                todoString: newTodo,
                completed:false
            });
        },
        toggleTodo(todo){
            todo.completed = !todo.completed;
        },
        editTodo(todo, newTodoString){
            todo.todoString = newTodoString;
        },
        deleteTodo(deleteTodo){
            this.todos = this.todos.fiter(todo => todo.todoString !== deleteTodo.todoString)
        },
        }
}
</script>
<style>
body{
  background-color: rgb(26,26,26);
  color: aliceblue;
}
</style>