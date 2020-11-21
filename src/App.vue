<template>
<div >
  <Todos id="app" v-bind:todos="todos"/>
</div>

</template>

<script>
import Todos from './components/Todos';

export default {
  name: 'App',
  components: {
    Todos
  },
  data() {
    return {
      todos: [
        {
          id:1,
          name: 'todo 1',
          completed: false,
        },
         {
          id:2,
          name: 'todo 2',
          completed: true,
        },
         {
          id:3,
          name: 'todo 3',
          completed: false,
        }
      ]
    }
  }
}
</script>

<style>
* {
box-sizing: border-box;
margin: 0;
padding: 0;
}

body {
font-family:Arial, Helvetica, sans-serif;
line-height: 1.4;
}
</style>
