<template>
    <div class="user-info">
      <h2>{{ title }}</h2>
      <p><strong>Nombre:</strong> {{ name }}</p>
      <p><strong>Descripción:</strong> {{ description }}</p>
    </div>
  </template>
  
  <script>
  export default {
    name: "UserInfo",
    data() {
      return {
        title: "Información del Usuario",
        name: "Jersson Fabián Buitrago Murcia",
        description: "Estudiante de Ingeniería de Sistemas V semestre 2024a-Corhuila."
      };
    }
  };
  </script>
  
  <style scoped>
  .user-info {
    padding: 15px;
    border: 1px solid #ccc;
    border-radius: 8px;
    max-width: 400px;
    margin: 10px auto;
  }
  </style>
  