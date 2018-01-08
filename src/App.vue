<template>
  <div id="app">
    <!-- Render the TodoList component -->
    <!-- TodoList becomes -->
    <todo-list></todo-list>
  </div>
</template>

<script>
import TodoList from './components/TodoList';

export default {
    name: 'app',
    components: {
        // Add a reference to the TodoList component in the components property
        TodoList
    }
};
</script>

<style>
#app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    color: #2c3e50;
    margin-top: 60px;
}
</style>
