<template>
    <ion-page :class="{ 'xxx-cls': toggle }">
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
import { ref, onMounted } from 'vue';
import { IonContent, IonHeader, IonPage, IonTitle, IonToolbar, IonButtons, IonBackButton } from '@ionic/vue';

const toggle = ref(false);

onMounted(() => {
  setTimeout(() => {
    toggle.value = true;
  });
});
</script>
  