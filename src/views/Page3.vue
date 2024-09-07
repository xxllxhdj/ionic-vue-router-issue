<template>
    <ion-page>
      <ion-header>
        <ion-toolbar>
          <ion-buttons slot="start">
              <ion-back-button/>
          </ion-buttons>
          <ion-title>Page 3</ion-title>
        </ion-toolbar>
      </ion-header>
      <ion-content>
        <div @click="$router.go(-1)">Back</div>
        <div @click="$router.go(-3)">Done</div>
      </ion-content>
    </ion-page>
</template>

<script setup lang="ts">
import { IonContent, IonHeader, IonPage, IonTitle, IonToolbar, IonButtons, IonBackButton } from '@ionic/vue';
</script>