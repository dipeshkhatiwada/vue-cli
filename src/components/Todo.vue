<template>
<li class="d-flex align-items-center list-group-item">{{todoString}}</li>
</template>

<script>
export default {
    props:{
        todoString: String,
        completed: Boolean
    },
    data(){
        return{
            isEditing: false,
            newTodoString:""
        }
    }
}
</script>

<style scoped>
.completed{
    text-transform: line-through;
}

</style>