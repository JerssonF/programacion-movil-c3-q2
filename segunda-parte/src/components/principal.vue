<template>
    <div class="app">
      <userinfo />
      <tasklist />
      <notification />
    </div>
  </template>
  
  <script>
  import userinfo from "./userinfo.vue";
  import tasklist from "./tasklist.vue";
  import notification from "./notification.vue";
  
  export default {
    name: "App",
    components: {
      userinfo,
      tasklist,
      notification
    }
  };
  </script>
  
  <style>
  .app {
    font-family: Arial, sans-serif;
    padding: 20px;
    text-align: center;
    display: flex;
    flex-direction: column;
    gap: 20px;
  }
  </style>
  