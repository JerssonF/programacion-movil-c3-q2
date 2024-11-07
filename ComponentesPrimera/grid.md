# Grid
Sistema de cuadrícula para organizar el diseño.

## Componente Grid.
```js
<template>
    <ion-grid>
      <ion-row>
        <ion-col>1</ion-col>
        <ion-col>2</ion-col>
        <ion-col>3</ion-col>
      </ion-row>
    </ion-grid>
  
    <ion-grid>
      <ion-row>
        <ion-col>1</ion-col>
        <ion-col>2</ion-col>
        <ion-col>3</ion-col>
        <ion-col>4</ion-col>
        <ion-col>5</ion-col>
        <ion-col>6</ion-col>
      </ion-row>
    </ion-grid>
  
    <ion-grid>
      <ion-row>
        <ion-col>1</ion-col>
        <ion-col>2</ion-col>
        <ion-col>3</ion-col>
        <ion-col>4</ion-col>
        <ion-col>5</ion-col>
        <ion-col>6</ion-col>
        <ion-col>7</ion-col>
        <ion-col>8</ion-col>
        <ion-col>9</ion-col>
        <ion-col>10</ion-col>
        <ion-col>11</ion-col>
        <ion-col>12</ion-col>
      </ion-row>
    </ion-grid>
  </template>
  
  <script lang="ts">
    import { IonCol, IonGrid, IonRow } from '@ionic/vue';
    import { defineComponent } from 'vue';
  
    export default defineComponent({
      components: { IonCol, IonGrid, IonRow },
    });
  </script>
  
  <style scoped>
    ion-col {
      background-color: #135d54;
      border: solid 1px #fff;
      color: #fff;
      text-align: center;
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

