<template>
    <div>
        <div v-bind:key="todo.id" v-for="todo in todos">
           <Todositem v-bind:todo="todo" v-on:del-todo="$emit('del-todo',todo.id)"/>
        </div>
    </div>
</template>

<script>
import Todositem from './TodosItem';
export default {
    name:"Todos",
    components:{
        Todositem
    },
    props:["todos"]
}
</script>

<style scoped>

</style>