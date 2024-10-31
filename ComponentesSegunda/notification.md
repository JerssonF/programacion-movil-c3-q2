# Notification.
Este componente muestra un mensaje de notificación con un título y un contenido.

## Componente Notification.
```js
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
  ```

 ## Vista
 
  ```js
  <template>
  <ion-page>
    <ion-header :translucent="true">
      <ion-toolbar>
        <ion-title>Blank</ion-title>
      </ion-toolbar>
    </ion-header>

    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Blank</ion-title>
        </ion-toolbar>
      </ion-header>

      <div id="container">
        <strong>Ready to create an app?</strong>
        <p>Start with Ionic <a target="_blank" rel="noopener noreferrer" href="https://ionicframework.com/docs/components">UI Components</a></p>
     
      </div>
   <userinfo></userinfo>
   <tasklist></tasklist> 
   <notification></notification> 
   <principal></principal> 
      
    </ion-content>
  </ion-page>
</template>

<script setup lang="ts">
import userinfo from '@/components/userinfo.vue';
import tasklist from '@/components/tasklist.vue';
import notification from '@/components/notification.vue';
import principal from '@/components/principal.vue';
import { IonContent, IonHeader, IonPage, IonTitle, IonToolbar } from '@ionic/vue';
</script>

<style scoped>
#container {
  text-align: center;
  
  position: absolute;
  left: 0;
  right: 0;
  top: 50%;
  transform: translateY(-50%);
}

#container strong {
  font-size: 20px;
  line-height: 26px;
}

#container p {
  font-size: 16px;
  line-height: 22px;
  
  color: #8c8c8c;
  
  margin: 0;
}

#container a {
  text-decoration: none;
}
</style>
```