<template>
  <div id="app">
    <!-- Render the TodoList component -->
    <!-- TodoList becomes -->
    <todo-list :todos="todos"></todo-list>
  </div>
</template>

<script>
import TodoList from './components/TodoList';

export default {
    name: 'app',
    components: {
        // Add a reference to the TodoList component in the components property
        TodoList
    },
    // data function avails data to the template
    data() {
        return {
            todos: [
                {
                    title: 'Todo A',
                    project: 'Project A',
                    done: false
                },
                {
                    title: 'Todo B',
                    project: 'Project B',
                    done: true
                },
                {
                    title: 'Todo C',
                    project: 'Project C',
                    done: false
                },
                {
                    title: 'Todo D',
                    project: 'Project D',
                    done: false
                }
            ]
        };
    }
};
</script>

<style>
#app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    color: #2c3e50;
    padding-top: 40px;
}
</style>
