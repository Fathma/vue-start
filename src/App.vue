<template> 
  <HelloWorld 
  title="Basic list"
  />
  <ButtonCom v-on:click="result" text="Add Task" color="green" />
  <TasksCom :tasks="tasks"/>
</template> 

<script>
import HelloWorld from './components/HelloWorld.vue'
import ButtonCom from './components/Button.vue'
import TasksCom from './components/Tasks.vue'


export default {
  name: 'App',
  components: {
    HelloWorld,
    ButtonCom,
    TasksCom
  },
  props:["result"],
  data() {
    return {
      tasks: [
        {
          id: 1,
          text: "study"
        },
        {
          id: 2,
          text: "study"
        },
        {
          id: 3,
          text: "study"
        },
      ]
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
