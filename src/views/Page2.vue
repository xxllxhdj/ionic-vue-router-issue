<template>
    <ion-page>
      <ion-header>
        <ion-toolbar>
          <ion-buttons slot="start">
              <ion-back-button/>
          </ion-buttons>
          <ion-title>Page 2</ion-title>
        </ion-toolbar>
      </ion-header>
      <ion-content>
        <ion-item>
          <ion-input label="Default input"></ion-input>
        </ion-item>
        <div @click="$router.push({ path: '/page3' })">Page 3</div>
        <div @click="$router.go(-2)">Done</div>
      </ion-content>
    </ion-page>
</template>

<script setup lang="ts">
import { IonContent, IonHeader, IonPage, IonTitle, IonToolbar, IonInput, IonItem, IonButtons, IonBackButton } from '@ionic/vue';
</script>