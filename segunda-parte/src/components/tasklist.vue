<template>
    <div class="task-list">
      <h3>{{ title }}</h3>
      <ul>
        <li v-for="task in tasks" :key="task">{{ task }}</li>
      </ul>
    </div>
  </template>
  
  <script>
  export default {
    name: "TaskList",
    data() {
      return {
        title: "Lista de Tareas",
        tasks: ["Realizar componentes agrupados", "realizar Manual", "Md con los códigos."]
      };
    }
  };
  </script>
  
  <style scoped>
  .task-list {
    padding: 15px;
    border: 1px solid #aaa;
    border-radius: 8px;
    max-width: 400px;
    margin: 10px auto;
  }
  ul {
    padding-left: 20px;
  }
  </style>
  