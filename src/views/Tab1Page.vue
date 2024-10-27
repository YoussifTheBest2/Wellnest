<template>
  <ion-page>
    <ion-header>

      <div class="page-header">

        <ion-grid>
          <ion-row>
            
            <div class="topbar-icon-container">
              <ion-icon class="icon" :icon="person"></ion-icon>
              <ion-icon class="icon" :icon="settings"></ion-icon>
            </div>

            <ion-col>
              <div class="img-container">
                <img src="/public/newlogo.png" class="mainpageimage" alt="" />
              </div>
            </ion-col>
            <ion-col>
              <div class="title-elements">
                <h3>Wellnest</h3>
                <p>Take care of yourself, one step at a time.</p>
              </div>
            </ion-col>
          </ion-row>
        </ion-grid>
      </div>
    </ion-header>

    <ion-content>
      <ion-grid>
        <ion-row>
          <ion-col>
            <a style="display: block; text-decoration: none; color: inherit;" href="./physicalhealth">
            <ion-card class="card-categories">
              <ion-card-header>
                <img src="/public/img1.png" alt="" />
              </ion-card-header>
              <ion-card-content>
                <center>
                  <ion-card-title>Physical Health</ion-card-title>
                </center>
              </ion-card-content>
            </ion-card>
          </a>
          </ion-col>

          <ion-col>
            

              <ion-card class="card-categories">
                <ion-card-header>
                  <img src="/public/img2.png" alt="" />
                </ion-card-header>
                <ion-card-content>
                  <center><ion-card-title>Mental Health</ion-card-title></center>
                </ion-card-content>
              </ion-card>
            
          </ion-col>
        </ion-row>

        <ion-row>
          <ion-col>
            <ion-card class="card-categories">
              <ion-card-header>
                <img src="/public/img4.png" alt="" />
              </ion-card-header>

              <ion-card-content>
                <center><ion-card-title>Social Health</ion-card-title></center>
              </ion-card-content>
            </ion-card>
          </ion-col>

          <ion-col>
            <ion-card class="card-categories">
              <ion-card-header>
                <img src="/public/img1.png" alt="" />
              </ion-card-header>

              <ion-card-content>
                <center>
                  <ion-card-title>Emotional Health</ion-card-title>
                </center>
              </ion-card-content>
            </ion-card>
          </ion-col>
        </ion-row>
      </ion-grid>
    </ion-content>
  </ion-page>
</template>

<script setup >

import { IonIcon } from '@ionic/vue';
import { book, logoIonic, person, settings } from 'ionicons/icons';
import { defineComponent } from 'vue';
import {
  IonPage,
  IonHeader,
  IonToolbar,
  IonTitle,
  IonContent,
} from "@ionic/vue";
import ExploreContainer from "@/components/ExploreContainer.vue";





</script>


<style>
:root {
  --ion-color-yellow: #f1ede1;
}

.page-header {
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  flex: wrap;
  position: relative;
}

.topbar-icon-container {
  position: absolute;
  right: 0;
}

.icon {
  font-size: x-large;
  opacity: 100%;

  margin: 0.415rem;
}

.title-elements {
  display: flex;
  justify-content: center;
  flex-direction: column;
  margin-top: 2rem;
}

.img-container {
  display: flex;
  justify-content: space-evenly;
  margin-top: 3rem;
}

.card-categories {
  min-height: 14rem;
}


.img-container img{
  width: 9rem;
  height: 9rem;
  border: #b7a87c solid 2px;
  border-radius: 30%;
}
</style>
