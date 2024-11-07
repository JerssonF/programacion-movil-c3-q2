# Card
Tarjeta para presentar información de forma visual.

## Componente Card.
```js
<template>
    <ion-card>
      <ion-card-header>
        <ion-card-title>Card Title</ion-card-title>
        <ion-card-subtitle>Card Subtitle</ion-card-subtitle>
      </ion-card-header>
  
      <ion-card-content>
        Here's a small text description for the card content. Nothing more, nothing less.
      </ion-card-content>
    </ion-card>
  </template>
  
  <script lang="ts">
    import { IonCard, IonCardContent, IonCardHeader, IonCardSubtitle, IonCardTitle } from '@ionic/vue';
    import { defineComponent } from 'vue';
  
    export default defineComponent({
      components: { IonCard, IonCardContent, IonCardHeader, IonCardSubtitle, IonCardTitle },
    });
  </script>
   ```

   ## Vista.

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
