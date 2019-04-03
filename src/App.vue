<template>
  <div id="app">
    <todo-list v-bind:todos="todos"></todo-list>
    
  </div>
</template>

<script>
import TodoList from './components/ToDoList'

export default {
  components: {
    TodoList,
  },
  data(){
    return {
      todos: [{
        title: 'To do A',
        project: 'Project A',
        done: false,
      },{
        title: 'To do B',
        project: 'Project B',
        done: true,
      },{
        title: 'To do C',
        project: 'Project C',
        done: false,
      },{
        title: 'To do D',
        project: 'Project D',
        done: false,
      }],
    };
  },
};
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: left;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
