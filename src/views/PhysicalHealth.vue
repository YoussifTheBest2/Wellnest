<template>
    <ion-page>
        <ion-header>

            <div class="page-header">


                <div class="topbar-icon-container-left">
                    <a href="/"><ion-icon class="icon" :icon="arrowBack"></ion-icon></a>

                </div>
                <div class="topbar-icon-container-right">
                    <ion-icon class="icon" :icon="person"></ion-icon>
              <ion-icon class="icon" :icon="settings"></ion-icon>
            
                </div>




                <div class="title-elements">
                    <h3>Physical Health</h3>
                </div>
            </div>
        </ion-header>

        <ion-content>
            <ion-grid>
                <ion-row>
                    <ion-col>
                        <ion-card class="ph-card-col" style="background-color: aqua;">
                            <ion-card-header></ion-card-header>
                            <ion-card-content></ion-card-content>
                        </ion-card>
                    </ion-col>

                    
                </ion-row>

                <ion-row>
                    <ion-col>
                        <ion-card class="ph-card-col" style="background-color: aqua;">
                            <ion-card-header></ion-card-header>
                            <ion-card-content></ion-card-content>
                        </ion-card>
                    </ion-col>
                </ion-row>
                <ion-row>
                    <ion-col>
                        <ion-card class="ph-card-col" style="background-color: aqua;">
                            <ion-card-header></ion-card-header>
                            <ion-card-content></ion-card-content>
                        </ion-card>
                    </ion-col>
                </ion-row>
                <ion-row>
                    <ion-col>
                        <ion-card class="ph-card-col" style="background-color: aqua;">
                            <ion-card-header></ion-card-header>
                            <ion-card-content></ion-card-content>
                        </ion-card>
                    </ion-col>
                </ion-row>
            </ion-grid>
        </ion-content>
    </ion-page>
</template>

<script setup>

import { IonIcon } from '@ionic/vue';
import { arrowBack, book, logoIonic, person, settings } from 'ionicons/icons';
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

.topbar-icon-container-left {
    position: absolute;
    left: 0;
}
.topbar-icon-container-right {
    position: absolute;
    right: 0;
}
.topbar-icon-container{
    margin: 10px;
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

.mainpageimg {
    width: 6rem;
    height: 6rem;
    border: black solid none;
}

.ph-card-col{
    min-height: 5rem;
}
</style>