<template>
    <ion-page>
      <ion-header>
        <ion-toolbar>
          <ion-buttons slot="start">
              <ion-back-button/>
          </ion-buttons>
          <ion-title>Page 1</ion-title>
        </ion-toolbar>
      </ion-header>
      <ion-content>
        <div @click="$router.push({ path: '/page2' })">Page 2</div>
      </ion-content>
    </ion-page>
</template>

<script setup lang="ts">
import { IonContent, IonHeader, IonPage, IonTitle, IonToolbar, IonButtons, IonBackButton } from '@ionic/vue';
</script>
  