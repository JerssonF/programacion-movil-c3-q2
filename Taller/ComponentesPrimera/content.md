# Content
Contenedor para organizar el contenido de la página.

## Componente Content.

```js
<template>
    <ion-header>
      <ion-toolbar>
        <ion-title> Header </ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content class="ion-padding">
      <h1>Heading 1</h1>
      <h2>Heading 2</h2>
      <h3>Heading 3</h3>
      <h4>Heading 4</h4>
      <h5>Heading 5</h5>
      <h6>Heading 6</h6>
  
      <p>Here's a small text description for the content. Nothing more, nothing less.</p>
    </ion-content>
    <ion-footer>
      <ion-toolbar>
        <ion-title> Footer </ion-title>
      </ion-toolbar>
    </ion-footer>
  </template>
  
  <script lang="ts">
    import { IonContent, IonFooter, IonHeader, IonTitle, IonToolbar } from '@ionic/vue';
    import { defineComponent } from 'vue';
  
    export default defineComponent({
      components: { IonContent, IonFooter, IonHeader, IonTitle, IonToolbar },
    });
  </script>
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
        <color></color>
        <icons></icons>
        <badge></badge>
        <card></card>
        <checkbox></checkbox>
        <chip></chip>
        <content></content>
        <custom></custom>
        <grid></grid>  
        <item></item>    
        
      </ion-content>
    </ion-page>
  </template>
  <script setup lang="ts">
  import icons from '@/components/icons.vue';
  import badge from '@/components/badge.vue';
  import card from '@/components/card.vue';
  import checkbox from '@/components/checkbox.vue';
  import chip from '@/components/chip.vue';
  import content from '@/components/content.vue';
  import custom from '@/components/custom.vue';
  import color from '@/components/color.vue';
  import grid from '@/components/grid.vue';
  import item from '@/components/item.vue';
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



