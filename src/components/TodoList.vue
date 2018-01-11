<template>
  <div>
    <!-- JavaScript expressions in Vue are enclosed in double curly brackets. -->
    <p>Completed Tasks: {{todos.filter(todo => {return todo.done === true}).length}}</p>
    <p>Pending Tasks: {{todos.filter(todo => {return todo.done === false}).length}}</p>
    <todo v-for="(todo, index) in todos" :todo="todo" :key="index"></todo>
  </div>
</template>

<script type = "text/javascript" >
import Todo from './Todo';
export default {
    props: ['todos'],
    components: {
        Todo
    }
};
</script>
<style>

</style>
