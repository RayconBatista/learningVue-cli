<template>
  <div id="app" class="comp">
    <h1> | {{ title }} |</h1>
    <p>Bem vindo</p>
    <teste-component></teste-component>
    <br>
    <form-component></form-component>
    <hr>
    <task-components></task-components>
  </div>
</template>

<script>
import testeComponent from "./components/testeComponent";
import formComponent from "./components/formComponent";
import taskComponents from "./components/taskComponents";

export default {
  name: 'app',
  components: {
    testeComponent,
    formComponent,
    taskComponents
  },
  data()
  {
    return{
      title: 'app component'
    }
  }
}
</script>

<style>

.comp{
  background-color: #42b983;
  border: 1px solid blue;
  margin: 5px;
  padding: 5px;
}


#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
