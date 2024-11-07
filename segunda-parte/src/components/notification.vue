<template>
    <div class="notification">
      <h4>{{ title }}</h4>
      <p>{{ message }}</p>
    </div>
  </template>
  
  <script>
  export default {
    name: "Notification",
    data() {
      return {
        title: "Notificación",
        message: "Tienes una nueva notificación importante. ¡Pasaste Progrmación Móvil!"
      };
    }
  };
  </script>
  
  <style scoped>
  .notification {
    padding: 15px;
    border: 1px solid #bbb;
    border-radius: 8px;
    max-width: 400px;
    margin: 10px auto;
    background-color: #cfc2c2;
  }
  </style>
  